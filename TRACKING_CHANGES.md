
here’s the LaTex package you can use to track changes by you and your co-author(s):

just type \usepackage{changes} at the beginning of your LaTex document (where all the other \usepackage{} commands are).

you can also set a different color from blue to track the changes by writing this command in the preamble (below the \usepackage{} commands): 

\colorlet{Changes@Color}{red}

then, when you and your coauthor(s) make changes in the document, you use \added{test} to add text (e.g. here it is just “test”). and \deleted{test} to delete text (here I delete “test”).

this way, both added and deleted text are marked-up as red text (similar to Word).

if you just want to accept all changes made by your coauthor(s), you can simply add [final] to the changes package:

\usepackage[final]{changes}

and if you want to reverse it, you can just delete [final] and you can see all changes again.

alternatively, there is another package for which you have already a template with examples on Overleaf (just log in over the link and you have the template there): 

https://www.overleaf.com/latex/examples/track-changes-in-latex-with-trackchanges/cymjcmjsnphy

