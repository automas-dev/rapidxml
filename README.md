# rapidxml

A CMake port of http://rapidxml.sourceforge.net/


## Usage


### Find Package

```sh
git clone https://gitlab.com/automas-dev/rapidxml
cd rapidxml
cmake -S . -B build
cmake --build build --target install
```

CMakeLists.txt

```cmake
find_package(rapidxml REQUIRED)

target_link_libraries(${TARGET} rapidxml::rapidxml)
```

main.cpp

```cpp
#include <rapidxml/rapidxml.hpp>
```


### Submodule

```sh
git submodule add https://gitlab.com/automas-dev/rapidxml.git
```

CMakeLists.txt

```cmake
add_subdirectory(rapidxml)

target_link_libraries(${TARGET} rapidxml::rapidxml)
```

