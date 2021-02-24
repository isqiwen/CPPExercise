cmake_minimum_required(VERSION 3.10)

# set the project name
project(CPPExercise VERSION 1.0)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# add header files
# g++ -I
include_directories(include)

# add library files
# g++ -L
link_directories(lib)

# set source files
set(SOURCE_FILES src/*.cpp)

# add the executable

# 1. test sizeof
add_executable(SizeOf src/size_of.cpp)

# 2. test variadic_templates
add_executable(VariadicTemplates src/variadic_templates.cpp)

# 3. test polymorphic
add_executable(Polymorphic src/polymorphic.cpp)

# 4. test lambda
add_executable(Lambda src/lambda.cpp)

# 5. test function pointer
add_executable(FuncPointer src/func_pointer.cpp)

# 6. test pointer
add_executable(Pointer src/pointer.cpp)