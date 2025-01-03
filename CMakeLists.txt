cmake_minimum_required(VERSION 3.10)
project(db_backup_cli)

set(CMAKE_CXX_STANDARD 17)

# Add source files
set(SOURCE_FILES
    src/main.cpp
    src/backup.cpp
    src/backup.h
    src/db_connection.cpp
    src/db_connection.h
    src/storage.cpp
    src/storage.h
    src/logger.cpp
    src/logger.h
    src/scheduler.cpp
    src/scheduler.h
    src/utils/compression.cpp
    src/utils/compression.h
    src/utils/notifications.cpp
    src/utils/notifications.h
)

add_executable(db_backup_cli ${SOURCE_FILES})