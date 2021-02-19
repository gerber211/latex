## Revision text highlight 
Use for journal paper revision to change the color of text
```latex
\usepackage{xcolor}                 % For revision text 
\definecolor{rt}{RGB}{184, 15, 10}  % Crimson
```
Sample usage:
```latex
Traditional multirotors \textcolor{revred}{(quadrotors, hexarotors, etc.)} are a type of ... 
```
Which results in something like:

Note: The "RGB" tag of the `\definecolor` can instead be written in lowercase as "rgb" in which case the color definition needs to be scaled \[0,1\] like:
```latex
\definecolor{revred}{rgb}{0.72, 0.06, 0.04}
```

##