default: book

book: main.tex auxiliary/biblio.bib auxiliary/preamble_book.tex
	pdflatex -shell-escape main.tex
	bibtex main
	pdflatex -shell-escape main.tex
	pdflatex -shell-escape main.tex
	mv main.pdf ASTR506_Notes.pdf
	open ASTR506_Notes.pdf
clean:
	rm -f *.log *.aux *.dvi
