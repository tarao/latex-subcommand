.SUFFIXES: .pdf .dvi .tex

.tex.dvi:
	platex $*

.dvi.pdf:
	platex $*
	dvips -f $< | ps2pdf - $@

object: object.pdf
object.dvi: object.tex
object.pdf: object.dvi
