main: main.aux Bibliography.bib main.bbl
	pdflatex main.tex; pdflatex main.tex

main.bbl: main.aux main.aux
	bibtex main.aux

main.aux:
	pdflatex main.tex


clean:
	find -iname \*.log \
	  -o -iname *.aux\
	  -o -iname \*.out\
	  -o -iname \*.bbl\
	  -o -iname \*.log\
	  -o -iname \*.blg\
	  -o -iname \.\*.swp\
	  -o -iname \*.xml\
	  |xargs rm 

.PHONY: main.aux
