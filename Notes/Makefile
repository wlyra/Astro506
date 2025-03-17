default: book

book: main.tex auxiliary/biblio.bib auxiliary/preamble_book.tex chapters/chapter1.tex chapters/chapter2.tex chapters/chapter3.tex chapters/chapter4.tex chapters/chapter5.tex chapters/chapter6.tex chapters/chapter7.tex
	pdflatex -shell-escape main.tex
	bibtex main
	pdflatex -shell-escape main.tex
	mv main.pdf ASTR506_Notes.pdf
	open ASTR506_Notes.pdf
clean:
	rm -f *.log *.aux *.dvi
