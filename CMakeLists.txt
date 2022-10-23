cmake_minimum_required(VERSION 3.17)
project(parser)

set(CMAKE_CXX_STANDARD 20)

add_library(simpleparser_internals
            Tokenizer.cpp
            Tokenizer.hpp
            Parser.cpp
            Parser.hpp
            FunctionDefinition.cpp
            FunctionDefinition.hpp
            Type.cpp Type.hpp
            Statement.hpp
            Statement.cpp)

add_executable(simpleparser main.cpp)

target_link_libraries(simpleparser simpleparser_internals)