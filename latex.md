## Revised text color change
Use for journal paper revision to change the color of text
```latex
\usepackage{xcolor}                 % For revision text 
\definecolor{rt}{RGB}{184, 15, 10}  % Crimson
```
Sample usage:
```latex
Traditional multirotors \textcolor{revred}{(quadrotors, hexarotors, etc.)} are a type of ... 
```
Which results in:\
![alt text](https://github.com/gerber211/latex/blob/main/redText.PNG?raw=true)

Note: The "RGB" tag of the `\definecolor` can instead be written in lowercase as "rgb" in which case the color definition is scaled \[0,1\] like:
```latex
\definecolor{revred}{rgb}{0.72, 0.06, 0.04}
```

## Revision text highlight
Use for journal paper revision to highlight text
```latex
\usepackage{color,soul}                 % For text highlights
\definecolor{lightGRN}{rgb}{.75,1,.75}  % Define a new color, in this case light green
\sethlcolor{lightGRN}                   % Set the \hl{} tag color to be lightGRN, as defined above
```
Which results in:\
![alt text](https://github.com/gerber211/latex/blob/main/grnHighlight.PNG?raw=true)
