.PHONY: componentize build-component

all: build-component

componentize:
	rm -rf wit_world/
	uvx componentize-py --wit-path component.wit --world adder bindings .


build-component:
	uvx componentize-py \
		--wit-path component.wit \
		--world adder \
		componentize \
		app \
		-o add.wasm
