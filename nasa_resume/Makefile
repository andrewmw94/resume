filename=resume

objects = $(filename).pdf $(filename).aux $(filename).log $(filename).out $(filename).bbl $(filename).blg $(filename).fls $(filename).fdb_latexmk


TEX=pdflatex
BIBTEX=bibtex
BUILDTEX=$(TEX) $(filename).tex

all:
	$(BUILDTEX)
	$(BIBTEX) $(filename)
	$(BUILDTEX)
	$(BUILDTEX)

clean:
	rm -f $(objects)
