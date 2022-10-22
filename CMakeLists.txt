
cmake_minimum_required(VERSION 3.17)
project(parser)

set(CMAKE_CXX_STANDARD 20)

add_executable(parser main.cpp Tokenizer.cpp Tokenizer.hpp Parser.cpp Parser.hpp FunctionDefinition.cpp FunctionDefinition.hpp Type.cpp Type.hpp Statement.cpp Statement.hpp)