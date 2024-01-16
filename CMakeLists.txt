# 设置CMake最低版本要求
cmake_minimum_required(VERSION 3.10)

# 设置项目名称
project(RISCV-IOT)

# 导入include目录中的头文件
include_directories(include)

# 获取src目录下的所有源文件
file(GLOB SOURCES "src/*.cpp")

# 为源文件生成一个可执行文件
add_executable(RISCV-IOT ${SOURCES})