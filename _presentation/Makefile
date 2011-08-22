install: rm_pdf copy_styles make_bibliography make_pdf clean
	evince _presentation.pdf &

make_pdf:
	pdflatex -shell-escape _presentation
	pdflatex -shell-escape _presentation

make_bibliography:
#	pdflatex -shell-escape _presentation
#	bibtex _presentation
#	pdflatex -shell-escape _presentation
#	pdflatex -shell-escape _presentation

rm_pdf:
	rm -f _presentation.pdf

copy_themes:
	mkdir -p ~/texmf/tex/latex/beamer
	cp -r themes/*.sty ~/texmf/tex/latex/beamer

copy_styles:
	mkdir -p ~/texmf/tex/latex/beamer
	cp -r stys/*.sty ~/texmf/tex/latex/beamer

clean:
	rm -f *.aux
	rm -f *.bbl
	rm -f *.bak
	rm -f *.log
	rm -f *.blg
	rm -f *.toc
	rm -f *.lot
	rm -f *.lof
	rm -f *.dvi
	rm -f *.idx
	rm -f *.ilg
	rm -f *.ind
	rm -f **/*~
	rm -f *~
	rm -f _presentation.ps
	rm -f _presentation.dvi
	rm -f *.nav
	rm -f *.out
	rm -f *.snm
	rm -f _presentation.pyg
	rm -f _presentation.vrb

