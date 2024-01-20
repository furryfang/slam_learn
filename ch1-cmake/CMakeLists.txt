cmake_minimum_required( VERSION 2.8 )
project( helloSlam )

set( CMAKE_BUILD_TYPE "Debug" ) # 设置为调试模式

add_executable( helloslam main.cpp ) # 编译cpp文件为可执行文件

add_library( helloslamlib lib_hello.cpp) # 编译cpp为.a库文件
target_link_libraries( helloslam helloslamlib ) # 将库文件链接到可执行文件中

