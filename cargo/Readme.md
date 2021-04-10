
These are minimal Cargo files that DO NOT
have plugins or features.  Just the core build.

This is a description of the changes to the Cargo.toml
file that happen to minimize the file...

Starting at line 32 all of the plugins get removed below

### nu-value-ext

The default features below rustyline-support get removed including:

* match
* post
* fetch
* zip-support

All of the extra and wasi get removed along with

### everything with the word plugin

### The following three things can stay.

* trash-support
* zip-support
* table-pager
