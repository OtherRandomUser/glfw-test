# GLFW Test Project

Just a GLFW project template

## Installation

On Ubuntu, first install the dependencies:

```bash
$ sudo apt install -y libx11-dev libxrandr-dev libxinerama-dev  libxcursor-dev libxi-dev mesa-common-dev
```

and then compile:

```bash
$ git submodules update --recursive
$ mkdir build && cd build
$ cmake ..
$ cmake --build . --parallel
```
