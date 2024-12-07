set(CMAKE_CXX_STANDARD 20)



set(CMAKE_CXX_FLAGS "-march=x86-64-v3")
set(CMAKE_C_FLAGS "-march=x86-64-v3")
set(CMAKE_LD_FLAGS "-march=x86-64-v3")

# take care of the main executable
add_executable(Gigantua
        Chess_Base.hpp
        Chess_Test.hpp
        Gigantua.cpp
        Movegen.hpp
        Movelist.hpp
        Movemap.hpp
)
