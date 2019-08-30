all: copy_theme
	pdflatex -halt-on-error 2019.08.30.tex
	pdflatex -halt-on-error 2019.08.30.tex

copy_theme:
	ln -snf ../UW-Theme/beamercolorthemeWisconsin.sty .
	ln -snf ../UW-Theme/beamercolorthemeWisconsinWhite.sty
	ln -snf ../UW-Theme/beamerouterthemesubtle.sty
	ln -snf ../UW-Theme/beamerthemeWisconsin.sty
	ln -snf ../UW-Theme/UW_crest.pdf
	ln -snf ../UW-Theme/UW_main_compact.pdf
	ln -snf ../UW-Theme/UW_main_compact_white.pdf
	ln -snf ../UW-Theme/UW_main.pdf
	ln -snf ../UW-Theme/UW_main_white.pdf
