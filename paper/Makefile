LATEX = pdflatex
MAIN  = main

all:	$(MAIN).pdf

$(MAIN).pdf: 	$(MAIN).tex
#	$(LATEX) $(MAIN).tex 
#	bibtex $(MAIN)
	$(LATEX) $(MAIN).tex 
	$(LATEX) $(MAIN).tex 

clean:
	rm -f $(MAIN).aux
	rm -f $(MAIN).bbl
	rm -f $(MAIN).ps
	rm -f $(MAIN).pdf
	rm -f $(MAIN).blg
	rm -f $(MAIN).log
	rm -f *~

zip:	
	zip paper.zip $(MAIN).tex *.bib fig*.pdf Makefile apj.bst emulateapj.cls

view: 
	open $(MAIN).pdf &

