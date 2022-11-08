all: labo correction
	echo "done"
	

labo: *.tex
	pdflatex -shell-escape -jobname="instru_labo2" instru_labo2.tex
	pdflatex -shell-escape -jobname="instru_labo2" instru_labo2.tex
	

correction: *.tex
	pdflatex -shell-escape -jobname=instru_labo2_correction "\def\koriG{} \input{instru_labo2.tex}"
	pdflatex -shell-escape -jobname=instru_labo2_correction "\def\koriG{} \input{instru_labo2.tex}"
	
clean:
	rm -f instru_labo2_correction.pdf rm instru_labo2.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc *.fls *.fdb_latexmk
	
