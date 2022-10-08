# docker-cmake

The image offers the same functionality as cmake ([documentation](https://cmake.org/documentation)).

## How to use this image
* Without parameters creates the default configuration
```
docker run -it --rm -v /_pathToCmakeListFolder_:/usr/src/Project -w /usr/src/Project/build marcusstuht/cmake:3.24.2-gcc-12.2.0
```
* Create configuration for release 
```
docker run -it --rm -v /_pathToCmakeListFolder_:/usr/src/Project -w /usr/src/Project/build marcusstuht/cmake:3.24.2-gcc-12.2.0 cmake -D CMAKE_BUILD_TYPE=Release ..
```
* Run build for configuration
```
docker run -it --rm -v /_pathToCmakeListFolder_:/usr/src/Project -w /usr/src/Project/build marcusstuht/cmake:3.24.2-gcc-12.2.0 cmake --build .
```
