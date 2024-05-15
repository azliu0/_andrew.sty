# _andrew.sty

my general use latex style file. the design takes inspiration from [Evan Chen](https://web.evanchen.cc/coursework.html), [Rachel Wu](https://people.csail.mit.edu/rmwu/notes.html), and [Andrew Lin](http://www.mit.edu/~lindrew/notes.html). 

this repository includes a minimal working example of a document that uses this style file, which showcases some functionality and demonstrates how to get things set up, in case you have never used a style file before. 

Examples of full notes using ```_andrew.sty``` can be found [here](https://azliu.cc/coursework). To see my workflow and how I use this style file, see [here](https://github.com/azliu0/dotfiles/tree/main/.config/latex).

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
