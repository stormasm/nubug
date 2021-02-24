```rust
for name in &sorted_names {
    if name.contains(' ') {
        println!("name with space = {}",name);
    } else {
        cmap.insert(name.to_owned(), Vec::new());
    };
}
```

#### List of subcommands
ansi strip   
autoenv trust   
autoenv untrust   
config clear   
config get   
config load   
config path   
config remove   
config set   
config set_into   
date format   
date list-timezone   
date now   
date to-table   
date to-timezone   
each group   
each window   
format filesize   
from csv   
from eml   
from ics   
from ini   
from json   
from ods   
from ssv   
from toml   
from tsv   
from url   
from vcf   
from xlsx   
from xml   
from yaml   
from yml   
group-by date   
hash base64   
keep until   
keep while   
math abs   
math avg   
math ceil   
math eval   
math floor   
math max   
math median   
math min   
math mode   
math product   
math round   
math stddev   
math sum   
math variance   
nu plugin   
path basename   
path dirname   
path exists   
path expand   
path extension   
path filestem   
path type   
random bool   
random chars   
random decimal   
random dice   
random integer   
random uuid   
roll column   
roll up   
rotate counter-clockwise   
seq date   
skip until   
skip while   
split chars   
split column   
split row   
str camel-case   
str capitalize   
str collect   
str contains   
str downcase   
str ends-with   
str find-replace   
str from   
str index-of   
str kebab-case   
str length   
str lpad   
str ltrim   
str pascal-case   
str reverse   
str rpad   
str rtrim   
str screaming-snake-case   
str snake-case   
str starts-with   
str substring   
str to-datetime   
str to-decimal   
str to-int   
str trim   
str upcase   
term size   
to csv   
to html   
to json   
to md   
to toml   
to tsv   
to url   
to xml   
to yaml   
url host   
url path   
url query   
url scheme   