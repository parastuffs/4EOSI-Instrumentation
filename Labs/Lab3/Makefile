all: labo correction
	echo "done"
	

labo: *.tex
	pdflatex -shell-escape -jobname="instru_labo3" instru_labo3.tex
	pdflatex -shell-escape -jobname="instru_labo3" instru_labo3.tex
	

correction: *.tex
	pdflatex -shell-escape -jobname=instru_labo3_correction "\def\koriG{} \input{instru_labo3.tex}"
	pdflatex -shell-escape -jobname=instru_labo3_correction "\def\koriG{} \input{instru_labo3.tex}"
	
clean:
	rm -f instru_labo3_correction.pdf rm instru_labo3.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk
	
