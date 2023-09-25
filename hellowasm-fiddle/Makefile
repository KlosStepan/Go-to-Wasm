# Define variables
GOROOT := $(shell go env GOROOT)

.PHONY: build

build:
	GOOS=js GOARCH=wasm go build -o main.wasm
	cp "$(GOROOT)/misc/wasm/wasm_exec.js" .

clean:
	# Remove build stuff; get back to "initial state"
	rm -rf go.sum main.wasm wasm_exec.js mybin