# Ueber LaTeX Templates

These are my Ueber LaTeX Templates. My main motivation to put them on GitHub is
so that I and my fellow students could use them together and reuse them for many
lectures, I will happily discuss improvements/pull requests as time permits
though.

## Usage

### Uebungsblatt

This is a template for Homework. The scructure of the parent directory should be
something like:

    ├── Uebung
    │   ├── 01_abgabe.tex
    │   ├── 01_aufgabe_1.tex
    │   ├── 01_aufgabe_2.tex
    │   └── _teilnehmer.tex
    ├── _templates
    │   └── Uebungsblatt.tex
    └── _title.tex

The `_title.tex` should contain the title of the lecture, `_teilnehmer.tex`
should contain the names of the people involved in the hand-in, the hand-ins
files are named `XX_abgabe.tex` where `XX` is the number of the hand-in and
`XX_aufgabe_Y.tex` contains the solution for exercise `Y` of the homework sheet
`XX`. `XX_abgabe.tex` then looks something like that:

    \input{../_templates/Uebungsblatt}
    
    \begin{document}
    \aufgabe{1}
    \aufgabe{2}
    \end{document}

## License

This software is provided under the MIT license:

Copyright (c) 2012 - Felix Schäfer

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
