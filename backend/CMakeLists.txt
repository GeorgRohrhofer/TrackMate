cmake_minimum_required(VERSION 3.20)
project(TrackMateBackend VERSION 0.1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)      # nützlich für clangd

find_package(Drogon REQUIRED)

include_directories(include)

file(GLOB_RECURSE APP_SOURCES
     "src/*.cpp")


add_executable(${PROJECT_NAME} ${APP_SOURCES})
target_link_libraries(${PROJECT_NAME} PRIVATE Drogon::Drogon)

# (optional) zusätzliche Warn‑ und Optimierungsflags
# target_compile_options(${PROJECT_NAME} PRIVATE -Wall -Wextra -O2)
