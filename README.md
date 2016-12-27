
A highly-experimental, largely-non-functional polyfill for WebAssembly.

I want to learn about the binary encoding and execution semantics of
WebAssembly, and trying to write a polyfill seemed like as good a way
to do it as any.  I make no promises about this ever turning into something
you'd want to use for Real Work.

We have:

* `wasm.js`:  the polyfill, the core of which is a hand-written parser for WASM
              that translates it into javascript for execution.

* `spec/`:  the https://github.com/WebAssembly/spec repo as a git submodule,
             to make it easy to run the tests.

* `Makefile`:  provides the following targets for your convenience:

  * `make test`:  run the full WebAssembly spec test suite
  * `make test TESTS=<pattern>`:  run specific tests from the suite


