
download:
	wget https://github.com/hakimel/reveal.js/archive/master.tar.gz
	tar -xzvf master.tar.gz
	mv reveal.js-master reveal.js
	rm master.tar.gz

clean:
	rm -rf reveal.js
	rm {{cookiecutter.output_file}}

build:
	pandoc -t revealjs -s -o {{cookiecutter.output_file}} {{cookiecutter.input_file}} -V revealjs-url=./reveal.js


.PHONY: clean download build
