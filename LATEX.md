## Revised text color change
Example:\
![alt text](https://github.com/gerber211/latex/blob/main/redText.PNG?raw=true)\
Preamble: 
```latex
\usepackage{xcolor}                           % To change color of text 
\definecolor{rt}{RGB}{184, 15, 10}            % Crimson, defined as RGB [0,255] value
% \definecolor{revred}{rgb}{0.72, 0.06, 0.04} % Crimson, defined as rgb [0,1] value
```
Note: Use *either* RGB or rgb—not both. Usage: 
```latex
Traditional multirotors \textcolor{revred}{(quadrotors, hexarotors, etc.)} are a type of ... 
```

## Revision text highlight
Example:\
![alt text](https://github.com/gerber211/latex/blob/main/grnHighlight.PNG?raw=true)\
Preamble:
```latex
\usepackage{color,soul}                   % For text highlights
\definecolor{lightGRN}{rgb}{.75, 1, .75}  % Define a new color, in this case light green
\sethlcolor{lightGRN}                     % Set the \hl{} tag color to be lightGRN, as defined above
```
Usage:
```latex
Traditional multirotors \hl{(quadrotors, hexarotors, etc.)} are a type of ... 
```

## Footnotes
Example:\
![alt text](https://github.com/gerber211/latex/blob/main/footnote1.PNG?raw=true)
and at the bottom of the column/page:\
![alt text](https://github.com/gerber211/latex/blob/main/footnote2.PNG?raw=true)
Preamble: None required in Overleaf.\
Usage:
```latex
Traditional multirotors\footnote{quadrotors, hexarotors, etc.} are a type of ...
```


