# Author: Javier Reyes

# Defines the name of the tex file
FILE=main

# Rule to update the pdf document based on the latex source and the bib reference file
$(FILE).pdf : $(FILE).tex chapters/titlepage.tex chapters/chapter1.tex chapters/chapter2.tex chapters/chapter3.tex chapters/chapter4.tex
	pdflatex $(FILE).tex
	biber $(FILE)
	pdflatex $(FILE).tex
	pdflatex $(FILE).tex

# Rule to clean the folder, deleting all the temporal files from the tex compilation
clean :
	find . \( -name "*.snm" -o -name "*.out" -o -name "*.nav" -o -name "*.aux" -o -name "*.bbl" -o -name "*.bcf" -o -name "*.blg" -o -name "*.lof" -o -name "*.log" -o -name "*.lot" -o -name "*.xml" -o -name "*.toc" -o -name "*.vrb" \) -delete

# temptempcommenttemptetetemp
