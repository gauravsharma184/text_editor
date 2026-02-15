cmake_minimum_required(VERSION 4.0.0)
project(text_editor VERSION 0.1.0 LANGUAGES C CXX)

add_subdirectory(cpp-terminal)

add_executable(text_editor main.cpp)

target_link_libraries(text_editor PRIVATE cpp-terminal)


set_property(TARGET text_editor PROPERTY CXX_STANDARD 17)


