cmake_minimum_required(VERSION 3.10)
project(3D-viewer)
set(CMAKE_CXX_STANDARD 17)
# Пошук бібліотек
find_package(glm CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
# Додавання виконуваного файлу
add_executable(3D-viewer src/main.cpp)
# Підключення бібліотек
target_link_libraries(3D-viewer PRIVATE glfw)
