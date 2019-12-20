TEXFILE := prelim

all:
	pdflatex $(TEXFILE)
	bibtex   $(TEXFILE)
	pdflatex $(TEXFILE)
	pdflatex $(TEXFILE)
	make clean

clean:
	rm -f $(TEXFILE).aux $(TEXFILE).bbl $(TEXFILE).blg  $(TEXFILE).idx \
          $(TEXFILE).lof $(TEXFILE).log $(TEXFILE).lot  $(TEXFILE).out \
          $(TEXFILE).toc

realclean: clean
	rm -f $(TEXFILE).pdf
