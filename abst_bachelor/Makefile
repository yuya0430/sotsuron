LATEX		= platex
DVIPS		= dvips
DVIPDF		= dvipdfmx
ENCODE		= utf8
SRC		= abst.tex
DVI		= $(SRC:.tex=.dvi)
PDF		= $(SRC:.tex=.pdf)

all:	$(PDF)


$(DVI):	$(SRC)
	$(LATEX) $(SRC)
	$(LATEX) $(SRC)
	$(LATEX) $(SRC)

$(PS):	$(DVI)
	$(DVIPS) -o $(PS) $(DVI)

$(PDF):	$(DVI)
	$(DVIPDF) -o $(PDF) $(DVI)

clean:;	\rm -f *.aux *.log $(DVI) $(PS) $(PDF)
