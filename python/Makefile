.PHONY: componentize build-component

all: component

bindings:
	rm -rf wit_world/
	uvx componentize-py --wit-path component.wit --world adder bindings .


component:
	uvx componentize-py \
		--wit-path component.wit \
		--world adder \
		componentize \
		app \
		-o add.wasm
