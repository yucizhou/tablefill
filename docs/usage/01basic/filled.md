<!-- This file was produced by 'tablefill.py'
	Template file: /home/mauricio/Documents/projects/dev/code/archive/2015/tablefill/docs/usage/01basic/template.md
	Input file(s): ['/home/mauricio/Documents/projects/dev/code/archive/2015/tablefill/docs/usage/01basic/input.txt']
To make changes, edit the input and template files.


DO NOT EDIT THIS FILE DIRECTLY.
 -->

<!-- tablefill:start tab:paragraph -->

Sample paragraph
- $N = 5,708$
- This is the 'tablefill example' sample.

Python-style formatting: 'python formatting'.

<!-- tablefill:end -->

<!-- tablefill:start tab:example -->

| Outcomes     | N    | Mean | (Std.) |
| ------------ | ---- | ---- | ------ |
| Outcomes 1 | 1,237 | 1.0 | (2.00) |
| Outcomes 2 | 2,234 | 3.0 | (2.40) |
| Outcomes 3 | 3 | 2.0 | (2.46) |
| Outcomes 4 | 2,234 | 3.0 | (2.40) |

<!-- tablefill:end -->

`pandoc` will compile raw LaTeX inside markdown documents, so
`tablefill` will also replace placeholders in LaTeX tables inside
markdown files. The replacement rules for LaTeX also apply here.

\begin{table}
  \caption{Table caption (e.g. regression results)}
  \label{tab:anotherExample}
  \begin{tabular}{p{4.25cm}c}
    Outcomes
    & Coef
    & (SE)
    \\
    Variable 1 & -1.2 (-1.18) \\
    Variable 2 & 2.8 (-0.53)*** \\
    Variable 3 & 1.1 (0.57)** \\
    \midrule
             N & 5,708 \\
    \multicolumn{4}{p{5cm}}{\footnotesize Footnotes!}
  \end{tabular}
\end{table}
\end{document}
