install: rm_pdf copy_styles make_bibliography make_pdf clean
	evince _sbc-template.pdf &

make_pdf:
	pdflatex -shell-escape _sbc-template
	pdflatex -shell-escape _sbc-template

make_bibliography:
	pdflatex -shell-escape _sbc-template
	bibtex _sbc-template
	pdflatex -shell-escape _sbc-template

rm_pdf:
	rm -f _sbc-template.pdf

copy_styles:
	mkdir -p ~/texmf/tex/latex/
	cp -r stys/*.sty ~/texmf/tex/latex/
	cp -r bsts/*.bst .

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
	rm -f _sbc-template.ps
	rm -f _sbc-template.dvi
	rm -f *.nav
	rm -f *.out
	rm -f *.snm
	rm -f _sbc-template.pyg
	rm -f _sbc-template.vrb
	rm -r *.bst

