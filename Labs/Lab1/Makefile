all: labo correction
	echo "done"
	

labo: *.tex
	pdflatex -shell-escape -jobname="instru_labo1" instru_labo1.tex
	pdflatex -shell-escape -jobname="instru_labo1" instru_labo1.tex
	

correction: *.tex
	pdflatex -shell-escape -jobname=instru_labo1_correction "\def\koriG{} \input{instru_labo1.tex}"
	pdflatex -shell-escape -jobname=instru_labo1_correction "\def\koriG{} \input{instru_labo1.tex}"
	
clean:
	rm -f instru_labo1_correction.pdf rm instru_labo1.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk
	
