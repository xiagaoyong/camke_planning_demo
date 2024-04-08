project(process)

add_library(${PROJECT_NAME} SHARED process.cpp)
include_directories(pnc_map)

target_include_directories(${PROJECT_NAME} PUBLIC ${PNC_Map_Dir})

target_link_libraries(${PROJECT_NAME} PUBLIC pnc_map)