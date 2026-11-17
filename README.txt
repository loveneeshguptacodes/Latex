LATEX FULL PRACTICAL PACK

Included:
- article.tex: article-class example with formatting, lists, tables, figure,
  equations, columns, labels/references, hyperlinks, citations, bibliography,
  and index.
- letter.tex: letter-class example with sender/recipient, date, opening,
  closing, signature and page setup.
- book.tex: book-class example with front/main/back matter, chapters,
  sections, contents, lists of figures/tables, figure, table, equations,
  appendix, index and references.
- references.bib: BibTeX database used by article.tex.
- workflow.png: image used by article.tex and book.tex.
- chapter-extra.tex: child file demonstrating \input.
- indic-language-examples.txt: practical workflow notes for Devanagari
  devnag and ITRANS.

COMPILE:
1) Article:
   pdflatex article.tex
   bibtex article
   makeindex article
   pdflatex article.tex
   pdflatex article.tex

2) Letter:
   pdflatex letter.tex

3) Book:
   pdflatex book.tex
   makeindex book
   pdflatex book.tex
   pdflatex book.tex

NOTE:
- Run commands from this folder.
- If the article has no index entries, MakeIndex may report an empty index;
  the command is included to demonstrate the workflow.
- The book demonstrates \input syntax in prose. To compile the separate
  child chapter, add \input{chapter-extra} in the main body before
  \appendix.
- Practical 8 and 9 require separate legacy preprocessors and font files;
  ordinary Overleaf Recompile does not automatically run devnag/ITRANS.
- Replace sample names and content as required by your practical question.
