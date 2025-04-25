# 源代码目录的CMakeLists.txt

# 添加库目标
add_library(connection_pool
    # 源文件将在这里添加
)

# 设置库的属性
target_include_directories(connection_pool
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
)

# 设置编译选项
target_compile_features(connection_pool PUBLIC cxx_std_17)