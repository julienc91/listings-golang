listings-golang
===============

This package provides Golang support for the `listings` package in LaTeX.

* Author: Julien CHAUMONT (https://julienc.io)
* Version: 1.1
* Date: 2017-10-11
* Licence: MIT
* Url: http://github.com/julienc91/listings-golang
* Golang version: 1.9

This version was adapted from the [golang-latex-listings][1] project.

## Usage

```latex

\documentclass[12pt,a4paper]{report}
\usepackage[utf8]{inputenc}
\usepackage{listings}
\usepackage{listings-golang} % import this package after listings
\usepackage{color}

\lstset{ % add your own preferences
    frame=single,
    basicstyle=\footnotesize,
    keywordstyle=\color{red},
    numbers=left,
    numbersep=5pt,
    showstringspaces=false, 
    stringstyle=\color{blue},
    tabsize=4,
    language=Golang % this is it !
}

\begin{document}
\begin{lstlisting}
package main

import "fmt"

func main() {
    fmt.Println("Hello World!")
}
\end{lstlisting}
\end{document}
```

Don't forget to put the file `listings-golang.sty` in the folder of your project,
or with the other installed packages.


  [1]: https://bitbucket.org/korfuri/golang-latex-listings
