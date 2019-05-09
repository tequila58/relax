# relax
Relax is a language for creating command-line websites (sort of)

# WIG
WIG stands for `Water Is Good` and is the equivalent of CSS.

# RIM
RIM stands for `Relax Interactive Module` and is responsible for the user being able to interact with the site.

# Cobalt/Cobaltium
Cobalt is a command-line browser that reads Relax, WIG and RIM code.
Cobaltium is the base for it, the core part of it, the language reader.
Cobaltium SrcView is an in-browser source code viewer.

# What's this thing written in?
Relax, WIG, RIM and Cobaltium are written in Crystal.

# Why Crystal?
Crystal is easy, sleek, fast and can compile to machine language.

# Syntax
Relax
```
[relax]
  [info]
    [wig] style.wig [.wig] // specifies directory of WIG code
    [rim] interact.rim [.rim] // specifies directory of RIM code
  [.info]
  [main] // main, equivalent of <body>
    [h mh]Hello![.h] // header with id "mh"
    [e.] // new line (empty space)
    [p]This is a simple page made in Relax - the command line website language[.p] // a paragraph
    [btn action="gtp2"]Click me![.btn] // a button with the action gtp2 (RIM)
  [.main]
[.relax]
```
WIG
```
relax
bgcolor gray // changes the background color to gray
relax

mh
font bold // changes the color to bold
mh
```
RIM
```
gtp2{
  ontype::click::goto example.com/page2 // if you type "click" you click the button gtp2 and you go to example.com/page2
}
```
