# Borrowed from github
# Change only the variable below to the name of the main tex file.
PROJNAME=resume


# The first rule in a Makefile is the one executed by default ("make"). It
# should always be the "all" rule, so that "make" and "make all" are identical.
all: $(PROJNAME).pdf

# MAIN LATEXMK RULE

# -pdf tells latexmk to generate PDF directly (instead of DVI).
# -use-make tells latexmk to call make for generating missing files.
# -pvc : Preview continuous mode, wont' work with Adobe
# -interactive=nonstopmode keeps the pdflatex backend from stopping at a
# missing file reference and interactively asking you for an alternative.

$(PROJNAME).pdf: $(PROJNAME).tex
	latexmk -pdf -pvc  $(PROJNAME).tex 


cleanall:
	latexmk -C

clean:
	latexmk -c
