# Hello, WebAssembly!
This is Go code compiled to Wasm for Hello World in simple VanillaJS website.
# Compile
```zsh
GOOS=js GOARCH=wasm go build -o main.wasm
cp "$(GOROOT)/misc/wasm/wasm_exec.js" .
```
See [Makefile](https://github.com/KlosStepan/Go-to-Wasm/blob/main/hellowasm-fiddle/Makefile).