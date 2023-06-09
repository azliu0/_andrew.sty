# _andrew.sty

general use latex style file. my design takes inspiration from [Evan Chen](https://web.evanchen.cc/coursework.html), [Rachel Wu](https://people.csail.mit.edu/rmwu/notes.html), and [Andrew Lin](http://www.mit.edu/~lindrew/notes.html). 

## features 

some features include: 
- a general style for writing handouts, as well as ```notes``` and ```pset``` options that can be used specifically for taking class notes and typing up problem sets
- a ```/importfiles``` command for note files so ```main.tex``` doesn't look like this:
```tex
% ...
\include{0527.tex}
\include{0603.tex}
\include{0610.tex}
\include{0617.tex}
\include{0624.tex}
\include{0701.tex}
\include{0708.tex}
\include{0715.tex}
\include{0722.tex}
% ...
```
- color boxes for pretty formatting
- templates for code boxes, asymptote/tikz configurations, and math symbols
