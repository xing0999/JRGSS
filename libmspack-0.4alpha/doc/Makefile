DOCS =	annotated.html classes.html files.html functions*.html globals*.html \
	jquery.js index.html mspack*.html struct*.html doxygen.* tab* search \
	*.png

all: index.html

clean:
	-rm -rf $(DOCS) installdox

index.html: ../mspack/mspack.h Doxyfile
	doxygen

mspack_docs.zip: index.html
	zip -9r $@ $(DOCS)
