# _andrew.sty

general use latex style file. this design takes inspiration from [Evan Chen](https://web.evanchen.cc/coursework.html), [Rachel Wu](https://people.csail.mit.edu/rmwu/notes.html), and [Andrew Lin](http://www.mit.edu/~lindrew/notes.html). This repository also contains an example file that can be copied for easy use. 

## features

* support for color boxes, as usual for most handouts. the specific color palette is viewable inside of ```_andrew.sty```.
* optional ```[notes]``` and ```[pset]``` arguments that specifically tailors the style for different purposes
* templates, including common matrix patterns (and block matrices), basic asymptote visuals, and table patters. useful for taking notes in real-time
* support for importing lots of files. when taking notes for various classes, I usually like to organize notes by lecture in different files (e.g., 0527.tex). instead of having ```main.tex``` look like this: 
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
the command ```\importfiles``` does everything for you. I made this command after realizing halfway through the semester that more than 75% of my ```main.tex``` was just importing files, and it was a bit of a hassle to have to scroll all the time.
