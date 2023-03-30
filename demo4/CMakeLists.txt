cmake_minimum_required (VERSION 3.0)

project (sqliteDemo)

aux_source_directory(. DIR_SRCS)

#指定生成目标
add_executable(Demo ${DIR_SRCS})

target_link_libraries(Demo LINK_PUBLIC sqlite3)
