CU_SET_PATH("CMAKE_MOD_STARTGUILD_DIR" "${CMAKE_CURRENT_LIST_DIR}")

AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/mod_startguild.cpp")

AC_ADD_SCRIPT_LOADER("StartGuild" "${CMAKE_CURRENT_LIST_DIR}/src/loader_startguild.h")

CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")