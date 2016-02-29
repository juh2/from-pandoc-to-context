all: example.pdf

example.pdf: example.xml
	contextjit --environment=exampleenv.tex example.xml

example.xml: example.md exampleenv.tex ../pandoc-xhtml.tex Makefile
	pandoc -S -s --html-q-tags --section-divs --gladtex -t html -o example.xml example.md