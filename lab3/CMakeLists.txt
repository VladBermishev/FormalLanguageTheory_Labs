project(lab3)
add_executable(${PROJECT_NAME} main.cpp)
add_library(${PROJECT_NAME}_lib INTERFACE)
target_include_directories(${PROJECT_NAME}_lib INTERFACE include)
target_link_libraries(${PROJECT_NAME} common ${PROJECT_NAME}_lib)