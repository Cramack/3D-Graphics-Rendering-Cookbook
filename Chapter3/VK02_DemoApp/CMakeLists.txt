cmake_minimum_required(VERSION 3.12)

project(Chapter3)

include(../../CMake/CommonMacros.txt)

include_directories(../../deps/src/vulkan/include)
include_directories(../../shared)

SETUP_APP(Ch3_SampleVK02_DemoApp "Chapter 03")

target_link_libraries(Ch3_SampleVK02_DemoApp PRIVATE glfw volk glslang SPIRV assimp SharedUtils)
