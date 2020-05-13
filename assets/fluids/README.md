<div align="center">

  <h1><code>Fast Fluid Dynamics</code></h1>

  <strong>Built with <a href="https://rustwasm.github.io/">Rust+WASM</a> and WebGL</strong>
</div>

## About
Sanjay Yepuri SSY365
Helen Zhou hpz76

For our final project we implemented an algorithm called Fast Fluid Dynamics (FFD) using Rust and WebGL. This is a method for creating real-time, stable fluid simulations that run entirely on the GPU based on Jos Stam’s paper, “Stable Fluids” (Stam 1999).

Our implementation is based on the tutorial in [this](https://developer.download.nvidia.com/books/HTML/gpugems/gpugems_ch38.html) GPU Gems Chapter.
## 🚴 Usage

### 🐑 Install dependencies

In order to use Rust and WASM you will need the nightly version of Rust. 
* First, install [rustup](https://rustup.rs/)
* Then, run the following commands to install the rust nightly toolchain and make it the default:
```
$ rustup install nightly
$ rustup default nightly
```
You will also need to install [Node.js](https://nodejs.org/en/). Then run the following command to install the javascript dependencies. 
```
$ npm install
```

### 🛠️ Build 
To build and run the project run the following command.
```
$ npm run serve
```
You can access the simulation from `localhost:3000`

To build without running the webserver execute: 
```
$ npm run build
```

### Project Structure 

The main source code is found in the `src` folder. The entrypoint is in `src/lib.rs`. This file creates the WebGL context and compiles and initializes all the necessary shader programs and buffer objects. It also contains the main render loop. `src/shaders` contains all the shader programs written in GLSL as well as some helper functions that load and compile the programs. Both `src/texture.rs` and `src/render.rs` are abstractions on top of webgl in order to simplify creating textures, renderbuffers, and render passes. These are similar to the classes found in the last animation project. The WebGL calls required to render to texture the velocity and pressures fields are put in helper functions found int `src/render_fluid.rs`. `gui.rs` contains the handlers mouse clicks on the canvas. 

The report is `report.pdf` and the presentation we used is exported as a pdf in `presentation.pdf`. We also included a few screen recordings.


### Extra Credit
Both Helen and I have submitted the ECIS instructure survey. 
## 🔋 Batteries Included

* [`wasm-bindgen`](https://github.com/rustwasm/wasm-bindgen) for communicating
  between WebAssembly and JavaScript.
* [`console_error_panic_hook`](https://github.com/rustwasm/console_error_panic_hook)
  for logging panic messages to the developer console.
* [`wee_alloc`](https://github.com/rustwasm/wee_alloc), an allocator optimized
  for small code size.
