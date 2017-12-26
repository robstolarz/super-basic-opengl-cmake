# simple

## build

* install linux
* install glfw from your package manager
* clone this repo
* run the following:

```
cd build
cmake ..
make
./testexec
```
the last command will return nothing, because it does nothing

(it will work on macOS with a tweak, and windows requires some manual care)

## why

this repo shows a nice way of using cmake and provides a quick starting point for potential glfw users

add new libraries by adding their FindXXX.cmake file to the cmake folder and using `find_package` on them as shown
