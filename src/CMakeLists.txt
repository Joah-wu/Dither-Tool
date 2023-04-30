find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(ImgTransfer
        main.cpp
        filesInfoGet.cpp
        imgProcess.cpp
        )
target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})
target_include_directories(ImgTransfer PUBLIC ${PROJECT_SOURCE_DIR}/inc)
