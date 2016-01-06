add_library(asio src/asio.cpp)

target_include_directories(asio PUBLIC include)
target_compile_definitions(asio PUBLIC "-DASIO_STANDALONE" "-DASIO_SEPARATE_COMPILATION")
set_target_properties(asio PROPERTIES FOLDER "External/asio")
