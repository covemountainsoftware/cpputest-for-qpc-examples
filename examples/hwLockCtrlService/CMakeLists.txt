include_directories(include)
add_subdirectory(test)
add_library(hwLockCtrlService include/hwLockCtrlService.h src/hwLockCtrlService.c)
target_link_libraries(hwLockCtrlService hwLockCtrl)
target_include_directories(hwLockCtrlService PUBLIC include)

# TODO: setting up QP should probably be a higher level build option
add_compile_definitions(QACTIVE_CAN_STOP)
include_directories(${QP_CPP_INCLUDE_DIR})
include(${CMS_CMAKE_DIR}/qpcPosixPortCMakeSupport.cmake)
