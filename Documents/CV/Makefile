all: latex_part 
	dvips -Ppdf -P cmz -Pdownload35 -j0 -G0 -t letter -o massem-cv.ps massem-cv.dvi
	ps2pdf14 -dPDFSETTINGS=/prepress -dEmbedAllFonts=true massem-cv.ps
	chmod 777 *.*
	make clean
latex_part:
	latex massem-cv; latex massem-cv; latex massem-cv;
massem-cv.pdf:
	ps2pdf massem-cv.ps massem-cv.pdf
clean:
	rm -f massem-cv.aux   massem-cv.bbl   massem-cv.blg  massem-cv.brf   massem-cv.dvi   massem-cv.log  massem-cv.ps massem-cv.out