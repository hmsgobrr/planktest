cmake_minimum_required(VERSION 3.0)
project(planktest C CXX)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

file(GLOB SOURCE "src/*.cpp" "src/*.h")
file(GLOB ASSETS
	"assets/*.png"
	"assets/*.jpg"
)

add_executable(${PROJECT_NAME} ${SOURCE} ${ASSETS})
