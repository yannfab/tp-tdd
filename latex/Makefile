CLEAN=*~ *.rtf *.ps *.log *.dvi *.aux *.pdf *.out *.html *.css *.bak *.toc *.pl *.4ct *.4tc *.lg *.sxw *.tmp *.xref *.idv *.tns
INIT=*.odt
CLS=*~ *.log *.aux *.out *.bak *.toc *.pl
TEXFILES = $(wildcard *.tex)
INPUTFILES = $(wildcard input/*.tex)
PSFILES = $(patsubst %.tex,%.ps,$(TEXFILES))

%.pdf: %.tex
	pdflatex  $<
	pdflatex  $<

clean:
	-rm -f $(CLEAN)

pdf: $(patsubst %.tex,%.pdf,$(TEXFILES)) 
