# dockerfile-emscripten-sdk

```
docker build . -t tfkd/emsdk
docker run -it --rm --name emcc-test -v "$PWD":/work tfkd/emsdk bash -c "./emccw /work/counter.c -s WASM=1 -s SIDE_MODULE=1 -o /work/counter.wasm"
```

This dockerfile is inspired by the blog below.

- http://blog.openbloc.fr/webassembly-first-steps/
