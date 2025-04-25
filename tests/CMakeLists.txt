# 测试目录的CMakeLists.txt

# 查找GTest包
find_package(GTest REQUIRED)

# 添加测试可执行文件
add_executable(connection_pool_tests
    # 测试源文件将在这里添加
)

# 链接测试库
target_link_libraries(connection_pool_tests
    PRIVATE
        connection_pool
        GTest::GTest
        GTest::Main
)

# 添加测试
add_test(NAME connection_pool_tests COMMAND connection_pool_tests)