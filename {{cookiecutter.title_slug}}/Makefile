
download-reveal-js:
	wget https://github.com/hakimel/reveal.js/archive/master.tar.gz
	tar -xzvf master.tar.gz
	mv reveal.js-master reveal.js
	rm master.tar.gz

clean:
	rm {{cookiecutter.output_file}}

clean-reveal-js:
	rm -rf reveal.js

build:
	pandoc -t revealjs -s -o {{cookiecutter.output_file}} {{cookiecutter.input_file}} -V revealjs-url=./reveal.js --slide-level 2


.PHONY: download-reveal-js clean build
