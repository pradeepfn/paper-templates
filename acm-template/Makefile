NAME = paper
TEX_SOURCES = $(NAME).tex 
BIB_FILES = ${NAME}.bib
EPS_FILES = figures/*

paper : $(TEX_SOURCES)
	pdflatex $(NAME)
	bibtex ${NAME}
	pdflatex $(NAME)
	pdflatex $(NAME)

clean:
	rm -f *.aux $(NAME).bbl $(NAME).blg $(NAME).log \
		$(NAME).dvi $(NAME).ps $(NAME).pdf
