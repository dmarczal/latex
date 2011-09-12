install: rm_pdf copy_styles make_pdf clean
	evince _ata_ciepe.pdf &

make_pdf:
	pdflatex -shell-escape _ata_ciepe
	pdflatex -shell-escape _ata_ciepe

rm_pdf:
	rm -f _ata_ciepe.pdf

copy_styles:
	mkdir -p ~/texmf/tex/latex/
	cp -r stys/*.sty ~/texmf/tex/latex/

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
	rm -f **/*.aux
	rm -f *~
	rm -f _ata_ciepe.ps
	rm -f _ata_ciepe.dvi
	rm -f *.nav
	rm -f *.out
	rm -f *.snm
	rm -f _ata_ciepe.pyg
	rm -f _ata_ciepe.vrb
	rm -f *.bst

