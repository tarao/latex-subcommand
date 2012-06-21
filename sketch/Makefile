.SUFFIXES: .pdf .dvi .tex

.tex.dvi:
	platex $*

.dvi.pdf:
	platex $*
	dvips -f $< | ps2pdf - $@

test: test.pdf
test.dvi: test.tex
test.pdf: test.dvi
