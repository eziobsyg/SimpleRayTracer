cmake_minimum_required(VERSION 3.10)  # 指定CMake的最低版本要求
project(RayTracingProject)            # 定义项目名称

# 设置C++标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 添加可执行文件
add_executable(RayTracing src/RayTracing.cpp) # 从RayTracing.cpp创建RayTracing.exe