# Solution: LaTeX Basics

Here's a complete solution for Exercise 1:

```latex
\documentclass{article}
\usepackage{amsmath}  % For mathematical notation
\usepackage{booktabs} % For professional tables

\title{My First LaTeX Document}
\author{Student Name}
\date{\today}

\begin{document}

\maketitle

\section{Introduction}
This is my first \LaTeX\ document. It demonstrates some \textbf{basic} formatting and \textit{structure} of a simple document. This paragraph contains both \textbf{bold text} and \textit{italic text}.

\subsection{Lists}
Here's a numbered list of my favorite programming languages:

\begin{enumerate}
    \item Python
    \item R
    \item MATLAB
    \item Julia
\end{enumerate}

And here's a bullet-point list of LaTeX benefits:

\begin{itemize}
    \item Professional typesetting
    \item Excellent math support
    \item Consistent formatting
    \item Free and open-source
\end{itemize}

\subsection{Tables}
Below is a simple table showing exam scores:

\begin{center}
    \begin{tabular}{lcr}
        \toprule
        Student & Subject & Score \\
        \midrule
        Alice & Mathematics & 95 \\
        Bob & Physics & 87 \\
        Charlie & Chemistry & 91 \\
        \bottomrule
    \end{tabular}
\end{center}

\end{document}
```



# Solution: Mathematical Typesetting

Here's a complete solution for Exercise 2:

```latex
\documentclass{article}
\usepackage{amsmath, amssymb}

\begin{document}

\section{Mathematical Expressions}

\subsection{Paragraph with Inline Math}
In mathematics, the symbol $\pi$ represents the ratio of a circle's circumference to its diameter, approximately $3.14159$. The famous Euler's identity states that $e^{i\pi} + 1 = 0$, which contains the fundamental constants $e$, $i$, $\pi$, $1$, and $0$. When solving quadratic equations of the form $ax^2 + bx + c = 0$, we use the formula $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.

\subsection{Displayed Equations}

An unnumbered equation:
\[
  E = mc^2
\]

A numbered equation:
\begin{equation}
  F = G\frac{m_1 m_2}{r^2}
\end{equation}

\subsection{Complex Equation with Fractions, Superscripts, Subscripts, and Greek Letters}

\begin{equation}
  \Delta S = k_B \log \left( \frac{\Omega_2}{\Omega_1} \right) = -k_B \sum_{i=1}^{n} p_i \log p_i
\end{equation}

\subsection{Piecewise Function using Cases}

\begin{equation}
  f(x) = 
  \begin{cases}
    x^2, & \text{if } x \geq 0 \\
    -x^2, & \text{if } x < 0
  \end{cases}
\end{equation}

\subsection{Matrix Equation}

\begin{equation}
  \begin{bmatrix}
    a & b \\
    c & d
  \end{bmatrix}
  \begin{bmatrix}
    x \\
    y
  \end{bmatrix}
  =
  \begin{bmatrix}
    ax + by \\
    cx + dy
  \end{bmatrix}
\end{equation}

\subsection{Multi-line Derivation with Alignment}

\begin{align*}
  (a + b)^2 &= (a + b)(a + b) \\
  &= a(a + b) + b(a + b) \\
  &= a^2 + ab + ba + b^2 \\
  &= a^2 + 2ab + b^2
\end{align*}

\end{document}
```


# Solution: Document Structure

Here's a complete solution for Exercise 3:

```latex
\documentclass{article}
\usepackage{amsmath, amssymb, amsthm}
\usepackage{graphicx}
\usepackage{booktabs}

% Define theorem-like environments
\newtheorem{theorem}{Theorem}[section]
\newtheorem{lemma}[theorem]{Lemma}

\theoremstyle{definition}
\newtheorem{definition}[theorem]{Definition}
\newtheorem{example}[theorem]{Example}

\title{Introduction to Vector Spaces}
\author{Student Name}
\date{\today}

\begin{document}

\maketitle
\tableofcontents

\section{Basic Definitions}

In this section, we introduce the fundamental concepts of vector spaces.

\begin{definition}\label{def:vectorspace}
A vector space $V$ over a field $F$ is a set equipped with two operations:
\begin{itemize}
    \item Addition: $+: V \times V \rightarrow V$
    \item Scalar multiplication: $\cdot: F \times V \rightarrow V$
\end{itemize}
satisfying the vector space axioms.
\end{definition}

\begin{example}\label{ex:r3}
The set $\mathbb{R}^3$ of all ordered triples $(x,y,z)$ with $x,y,z \in \mathbb{R}$ forms a vector space over $\mathbb{R}$ with the standard operations of component-wise addition and scalar multiplication.
\end{example}

\begin{figure}
    \centering
    \includegraphics[width=0.6\textwidth]{example-image-a}
    \caption{Geometric representation of vectors in $\mathbb{R}^3$}
    \label{fig:r3}
\end{figure}

As illustrated in Figure~\ref{fig:r3}, vectors in $\mathbb{R}^3$ can be visualized as arrows in 3D space.

\section{Linear Independence}

In this section, we explore the concept of linear independence.

\begin{theorem}\label{thm:lindep}
Let $V$ be a vector space and $\{v_1, v_2, \ldots, v_n\}$ be a set of vectors in $V$. These vectors are linearly independent if and only if the equation
\[
c_1 v_1 + c_2 v_2 + \ldots + c_n v_n = 0
\]
has only the trivial solution $c_1 = c_2 = \ldots = c_n = 0$.
\end{theorem}

\begin{table}
    \centering
    \caption{Dimensions of common vector spaces}
    \label{tab:dimensions}
    \begin{tabular}{lc}
        \toprule
        Vector Space & Dimension \\
        \midrule
        $\mathbb{R}^n$ & $n$ \\
        $\mathcal{P}_n$ (Polynomials of degree $\leq n$) & $n+1$ \\
        $M_{m,n}$ (Matrices of size $m \times n$) & $m \times n$ \\
        \bottomrule
    \end{tabular}
\end{table}

As shown in Table~\ref{tab:dimensions}, different vector spaces have different dimensions. The dimension of a vector space is related to the concept introduced in Theorem~\ref{thm:lindep}.

Referring back to Definition~\ref{def:vectorspace}, we can construct many examples similar to Example~\ref{ex:r3} by defining appropriate operations.

\end{document}
```

# Solution: Advanced Figures

Here's a complete solution for Exercise 5:

```latex
\documentclass{article}
\usepackage{graphicx}
\usepackage{tikz}
\usepackage{wrapfig}
\usepackage[margin=1in]{geometry}
\usepackage{lipsum}  % For dummy text

\title{Advanced Figure Techniques in LaTeX}
\author{Student Name}
\date{\today}

\begin{document}

\maketitle

\section{Side-by-Side Figures}

Figure arrangement is an important skill for creating professional documents. Below are two figures displayed side by side using the minipage environment.

\begin{figure}[ht]
    \centering
    % First figure
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=\textwidth]{example-image-a}
        \caption{First sample image showing concept A}
        \label{fig:side1}
    \end{minipage}
    \hfill
    % Second figure
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=\textwidth]{example-image-b}
        \caption{Second sample image showing concept B}
        \label{fig:side2}
    \end{minipage}
\end{figure}

As shown in Figures \ref{fig:side1} and \ref{fig:side2}, we can place images side by side while giving each its own caption and label. This arrangement is particularly useful when comparing related images.

\section{Grid of Figures}

For more complex arrangements, we can create a grid of figures. The following is a 2×2 grid of images:

\begin{figure}[ht]
    \centering
    % Top row
    \begin{minipage}{0.4\textwidth}
        \centering
        \includegraphics[width=0.9\textwidth]{example-image-a}
        \caption{Top-left image}
        \label{fig:grid1}
    \end{minipage}
    \hfill
    \begin{minipage}{0.4\textwidth}
        \centering
        \includegraphics[width=0.9\textwidth]{example-image-b}
        \caption{Top-right image}
        \label{fig:grid2}
    \end{minipage}
    
    \vspace{1cm}
    
    % Bottom row
    \begin{minipage}{0.4\textwidth}
        \centering
        \includegraphics[width=0.9\textwidth]{example-image-c}
        \caption{Bottom-left image}
        \label{fig:grid3}
    \end{minipage}
    \hfill
    \begin{minipage}{0.4\textwidth}
        \centering
        \includegraphics[width=0.9\textwidth]{example-image}
        \caption{Bottom-right image}
        \label{fig:grid4}
    \end{minipage}
\end{figure}

The four images in the grid (Figures \ref{fig:grid1}, \ref{fig:grid2}, \ref{fig:grid3}, and \ref{fig:grid4}) demonstrate how to organize multiple related figures in a structured layout.

\section{Annotated Figure with TikZ}

TikZ allows us to create sophisticated diagrams and to annotate images with precise control:

\begin{figure}[ht]
    \centering
    \begin{tikzpicture}
        % Base image
        \node[anchor=south west,inner sep=0] (image) at (0,0) {
            \includegraphics[width=0.8\textwidth]{example-image-a}
        };
        
        % Get the size of the image
        \begin{scope}[x={(image.south east)},y={(image.north west)}]
            % Overlay a smaller image
            \node at (0.75,0.75) {
                \includegraphics[width=0.25\textwidth]{example-image-b}
            };
            
            % Add arrows and annotations
            \draw[->,red,thick] (0.3,0.4) -- (0.5,0.5);
            \node[draw,fill=white,font=\small] at (0.2,0.4) {Key feature};
            
            \draw[->,blue,thick] (0.7,0.2) -- (0.6,0.3);
            \node[draw,fill=white,font=\small] at (0.8,0.15) {Detail};
            
            % Add circle highlight
            \draw[green,thick,dashed] (0.6,0.6) circle (0.1);
            \node[draw,fill=white,font=\small] at (0.75,0.6) {Region of interest};
        \end{scope}
    \end{tikzpicture}
    \caption{Annotated image with overlays, arrows, and callouts}
    \label{fig:annotated}
\end{figure}

Figure \ref{fig:annotated} demonstrates how to annotate an image with overlays, arrows, and text callouts using TikZ. This technique is particularly useful for highlighting specific features or explaining complex diagrams.

\section{Text Wrapping Around Figures}

Sometimes, it's desirable to have text wrap around a figure rather than placing the figure in its own block.

\begin{wrapfigure}{r}{0.5\textwidth}
    \centering
    \includegraphics[width=0.45\textwidth]{example-image-c}
    \caption{A figure with text wrapping around it}
    \label{fig:wrapped}
\end{wrapfigure}

\lipsum[1-2] % This generates dummy text that wraps around the figure

As shown in Figure \ref{fig:wrapped}, the wrapfig package allows text to flow naturally around images. This can save space and improve the visual flow of your document, especially for smaller illustrative figures that don't need to break the text completely.

\lipsum[3] % More dummy text

\section{Conclusion}

Advanced figure arrangements in LaTeX require careful planning but offer great flexibility in presenting visual information. The techniques demonstrated in this document can be combined and customized to suit various document types and presentation needs.

\end{document}
```