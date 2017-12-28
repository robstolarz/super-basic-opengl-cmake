# simple

## build

* install unix (macOS counts)
* install glfw from your package manager (macOS uses https://brew.sh)
* clone this repo
* run the following:

```
cd build
cmake ..
make
./testexec
```
the last command will return nothing, because it does nothing

(windows will work, but needs you to set paths to glfw)

## why

this repo shows a nice way of using cmake and provides a quick starting point for potential glfw users

add new libraries by adding their FindXXX.cmake file to the cmake folder and using `find_package` on them as shown
