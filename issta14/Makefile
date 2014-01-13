PAPER=paper

all: rubber #clean


grap:
	(cd graphs/; make)

cod:
	(cd code/; make)

pdf:
	pdflatex $(PAPER)
	bibtex $(PAPER)
	pdflatex $(PAPER)
	pdflatex $(PAPER)

rubber:
	rubber -d $(PAPER).tex

mk:
	latexmk -pvc -pdf $(PAPER).tex

clean:
	rm -f *.blg  *.bak *~ *.log *.aux *.bbl *_latexmk

distclean:
	rm -f $(PAPER).dvi $(PAPER).pdf $(PAPER).ps

