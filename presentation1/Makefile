PROJECT=main
TEX=pdflatex
BIBTEX=bibtex
BUILDTEX=$(TEX) $(PROJECT).tex
BUILDTEXDRAFT=$(TEX) -draftmode $(PROJECT).tex

all:
	$(BUILDTEXDRAFT)
	$(BIBTEX) $(PROJECT)
	$(BUILDTEXDRAFT)
	$(BUILDTEX)
clean-all:
	rm -f *.dvi *.log *.aux *.bbl *.blg *.idx *.ps *.eps *.pdf *.toc *.out *~ *.nav *.snm *.vrb
clean:
	rm -f *.log *.aux *.bbl *.blg *.idx *.toc *.out *~ *.nav *.snm *.vrb
