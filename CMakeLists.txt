project(DbTictactoe)

find_package(Qt5Core CONFIG REQUIRED)

set(HEADERS
)

set(SOURCES
    main.cpp
)

add_executable(tictactoe ${HEADERS} ${SOURCES})

target_link_libraries(tictactoe stdc++ Qt5::Core)
