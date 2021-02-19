## Common math
Example:\
![alt text](https://github.com/gerber211/latex/blob/main/generalMath.PNG?raw=true)\
Preamble: 
```latex
\usepackage{amsmath,amssymb,bm}   % Common math
```
Notes: These are the three most common math packages, included in a single call to `\usepackage{}`. The first two enable common math notation while the third, `bm`, enables __bold__ symbols for vector notation.\
Usage: 
```latex
Note that $d_e$ is the perpendicular distance from $\bm{c}_t$ to $\bm{p}_c$, calculated as
\begin{equation} \label{exampleEquation}
d_e = \left\lVert \left( \bm{a}_t-\bm{p}_c \right) - \left[\left(\bm{a}_t-\bm{p}_c\right) \cdot \bm{\hat{n}}_t \right] \bm{\hat{n}}_t \right\rVert
\end{equation}
where
$\bm{a}_t\in\mathbb{R}^{3}$ is any point on $\bm{c}_t$ and $\bm{\hat{n}}_t$ is a unit vector in the direction of $\bm{c}_t$.
```


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
![alt text](https://github.com/gerber211/latex/blob/main/footnote1.PNG?raw=true)\
and at the bottom of the column/page:\
![alt text](https://github.com/gerber211/latex/blob/main/footnote2.PNG?raw=true)\
Preamble: None required in Overleaf.\
Usage:
```latex
Traditional multirotors\footnote{quadrotors, hexarotors, etc.} are a type of ...
```

## Math symbols in text (textcomp)
Example:\
![alt text](https://github.com/gerber211/latex/blob/main/textcomp.PNG?raw=true)\
Preamble:
```latex
\usepackage{textcomp}
```
Usage:
```latex
The average retinal membrane thickness is 50\textpm5 \textmu m, 
while the average angle is 60\textdegree~without something.
```
Notes: This is arguably one of the most important packages to use as it produces math symbols outside of math mode. 
[The list of options](http://tug.ctan.org/info/symbols/comprehensive/symbols-a4.pdf) is extensive, but some of the most important are:
```latex
\textdegree   % The ° (degree) symbol
\textmu       % Greek lowercase µ
\textpm       % The ± (plus/minus) symbol
\texttimes    % The × (times) symbol
```
Note that `\textdegree` requires a `~` space after it and if you want to write µm, you need to use `\textmu m` (with a space). 

