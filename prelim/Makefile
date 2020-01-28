PDFLATEX := pdflatex -halt-on-error
BIBTEX   := bibtex

TEXFILE  := prelim

all:
	$(PDFLATEX) $(TEXFILE)
	$(BIBTEX)   $(TEXFILE)
	$(PDFLATEX) $(TEXFILE)
	$(PDFLATEX) $(TEXFILE)
	make clean

clean:
	rm -f $(TEXFILE).aux $(TEXFILE).bbl $(TEXFILE).blg  $(TEXFILE).idx \
          $(TEXFILE).lof $(TEXFILE).log $(TEXFILE).lot  $(TEXFILE).out \
          $(TEXFILE).toc

realclean: clean
	rm -f $(TEXFILE).pdf
