# relax
Relax is a language for creating command-line websites (sort of)

# WIG
WIG stands for `Water Is Good` and is the equivalent of CSS.

# RIM
RIM stands for `Relax Interactive Module` and is responsible for the user being able to interact with the site.

# Cobaltium
Cobaltium is the interpreter of Relax, WIG and RIM.

# What's this thing written in?
Relax, WIG, RIM and Cobaltium are written in Crystal.

# Why Crystal?
Crystal is easy, sleek, fast and can compile to machine language.

# Syntax
Relax
```
[wig] style.wig [.wig]
[rim] interact.rim [.rim]
[h id::mh]Hello![.h]
[e.]
[p]This is a simple page made in Relax - the command line website language[.p]
[btn action="gtp2"]Click me![.btn]
```
Let's deconstruct:
`[wig]` specifies the directory of the style of style.
`[rim]` specifies the directory of the interactive module
`[h id::mh]` creates a heading with the ID `mh`
`[e.]` new line
`[btn action::mbtn]` button with the RIM action `mbtn`

WIG
```
relax::start
font gray
relax::end

mh::start
font red
mh::end
```

RIM
```
gtp2::start
  ontype::click::goto example.com/page2
gtp2::end
```
