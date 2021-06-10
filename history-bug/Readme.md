
So every once in awhile the history file gets corrupted
and once this happens everything goes awry.

Step 1 is to try and figure out how to reproduce this problem.

Here are places where issues could be located.

Where is *LineResult* referenced ?

nu-cli/src/cli.rs
nu-cli/src/line_editor.rs
nu-engine/src/script.rs


In cli.rs when this happens --- when a **LineResult::Error** happens WHY is is the history updated ?  It seems to me that we should not be adding a history entry if an ERROR occurs.

So maybe the first thing to do is re-create a **LineResult::Error**

```.rust
LineResult::Error(line, err) => {
    if options.save_history && !line.trim().is_empty() {
        rl.add_history_entry(&line);
        let _ = rl.append_history(&history_path);
    }
```

#### The history -c -clear command is also broken
