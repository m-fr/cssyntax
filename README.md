[![Build Status](https://travis-ci.com/m-fr/cssyntax.svg?branch=master)](https://travis-ci.com/m-fr/cssyntax)

# CSSyntax
This is repository with C# syntax highlighter for TeX (OPmac).
The highlighter was made as part of semestral work for Typography and TeX course at FIT CTU.

You can see full documentation [in english](https://github.com/m-fr/cssyntax/releases/latest/download/doc-en.pdf) or [in czech](https://github.com/m-fr/cssyntax/releases/latest/download/doc-cz.pdf).
The highlighter itself is in file [cssyntax.tex](cssyntax.tex).

## Usage

You can paste whole macro into source document.
If you don't want to do this, you can just include file `cssyntax.tex`.
That can be done using `\input cssyntax`.

After inclusion of the macro you can use `\hisyntax{CS}` or `\ghisyntax{CS}` before verbatim to use highlighter locally or globally.
In source document the verbatim can look like this:
```
\hisyntax{CS}
\begtt
string foo = "bar";
...
\endtt
```