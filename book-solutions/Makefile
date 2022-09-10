# Currently only works with xelatex
LC=xelatex
LARGS=
DOWNLOAD_PROG=wget
DOWNLOAD_OPT=


all: build

build: index.tex
	@if [ ! -e Garamond-Math.otf ]; then\
		${DOWNLOAD_PROG} ${DOWNLOAD_OPT} "http://mirrors.ctan.org/fonts/garamond-math.zip"; \
		unzip -o garamond-math.zip; \
		mv garamond-math/Garamond-Math.otf .; \
		rm -Rf garamond-math{,.zip}; \
	fi
	${LC} ${LARGS} $^

clean:
	-rm Garamond-Math.otf
	-rm *.log index.pdf  *.aux