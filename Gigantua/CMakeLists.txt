set(CMAKE_CXX_STANDARD 20)


set(CMAKE_INTERPROCEDURAL_OPTIMIZATION TRUE)
set(CMAKE_VERBOSE_MAKEFILE on)

set(CMAKE_CXX_FLAGS "/clang:-O3 /clang:-march=x86-64-v3 /clang:-flto=auto")
set(CMAKE_C_FLAGS "/clang:-O3 /clang:-march=x86-64-v3 /clang:-flto=auto")
set(CMAKE_LD_FLAGS "/clang:-O3 /clang:-march=x86-64-v3 /clang:-flto=auto")

# take care of the main executable
add_executable(Gigantua
        Chess_Base.hpp
        Chess_Test.hpp
        Gigantua.cpp
        Movegen.hpp
        Movelist.hpp
        Movemap.hpp
)
