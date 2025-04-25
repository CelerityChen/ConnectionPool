# 示例目录的CMakeLists.txt

# 添加示例可执行文件
add_executable(connection_pool_example
    # 示例源文件将在这里添加
)

# 链接连接池库
target_link_libraries(connection_pool_example
    PRIVATE
        connection_pool
)