cmake_minimum_required(VERSION 3.10)  # 指定CMake的最低版本要求
project(RayTracingProject)            # 定义项目名称

# 设置C++标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

IF(${SOL})
	FILE(GLOB_RECURSE SOURCES "src0/*.cpp")
	FILE(GLOB_RECURSE HEADERS "src0/*.h")
ELSE()
	FILE(GLOB_RECURSE SOURCES "src/*.cpp")
	FILE(GLOB_RECURSE HEADERS "src/*.h")
ENDIF()

# 添加可执行文件
ADD_EXECUTABLE(${CMAKE_PROJECT_NAME} ${SOURCES} ${HEADERS}) # 从RayTracing.cpp创建RayTracing.exe