.PHONY: build clean
.DEFAULT_GOAL := build

OPTIMISE ?= yes

build:
	npm install
ifeq ($(OPTIMISE), yes)
	$(shell npm bin)/webpack --mode=production
else
	$(shell npm bin)/webpack --mode=development
endif

clean:
	rm -rf node_modules/
	rm -rf ../site/themes/i3camini/static/
