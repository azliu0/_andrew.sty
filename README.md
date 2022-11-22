# _andrew.sty
My general use latex style file. Stylistic inspiration for this design came from some combination of the notes of [Rachel Wu](https://people.csail.mit.edu/rmwu/notes.html), [Andrew Lin](http://www.mit.edu/~lindrew/notes.html), and [Evan Chen](https://web.evanchen.cc/coursework.html). See the MWE in this repository for a fast way to set up (compile multiple times with asymptote, LaTeX, etc. for everything to show properly if running locally). Examples of full-length projects compiled with ```_andrew.sty``` can be found [here](https://github.com/yellowtomato98/class-notes).

## features

* support for color boxes, as usual for most handouts. the specific color palette is viewable inside of ```_andrew.sty```.
* optional ```[notes]``` tag that specifically tailors the style file for taking notes in class (as opposed to e.g. writing handouts)
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

## features I want to add 
* support for theorem/corollary/proposition/etc. referencing tags. right now, the way that I've set up my color boxes is separate from the way that I'm tagging each box, meaning that referencing does not work like it normally would (i.e., for regular ```\begin{theorem} ... \end{theorem}``` 
environments). I'd like to try to combine these two functionalities
* create commands for some of my templates, so incorporating them in real-time is faster
