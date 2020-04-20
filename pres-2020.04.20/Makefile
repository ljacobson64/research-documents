TEXFILE := 2020.04.20

THEME_FILES := beamercolorthemeWisconsin.sty \
               beamercolorthemeWisconsinWhite.sty \
               beamerouterthemesubtle.sty \
               beamerthemeWisconsin.sty \
               UW_crest.pdf \
               UW_main_compact.pdf \
               UW_main_compact_white.pdf \
               UW_main.pdf \
               UW_main_white.pdf

all: copy_theme
	pdflatex -halt-on-error $(TEXFILE).tex
	pdflatex -halt-on-error $(TEXFILE).tex
	make clean

copy_theme:
	for f in $(THEME_FILES); do \
	  ln -snf ../UW-beamer-theme/$$f .; \
	done

clean:
	rm -f $(THEME_FILES) $(TEXFILE).aux $(TEXFILE).log $(TEXFILE).nav \
	      $(TEXFILE).out $(TEXFILE).snm $(TEXFILE).toc

realclean: clean
	rm -f $(TEXFILE).pdf
