AUX_SOURCE_DIRECTORY(./hello/src HELLO_LIB_CPP)
AUX_SOURCE_DIRECTORY(./sqrt/src  SQRT_LIB_CPP)
list(APPEND LIB_CPP ${HELLO_LIB_CPP} ${SQRT_LIB_CPP})
#message(STATUS "LIB_CPP = ${LIB_CPP}")
ADD_LIBRARY(hellosqrt SHARED ${LIB_CPP})

#LINK_DIRECTORIES(${LIBRARY_OUTPUT_PATH})
#AUX_SOURCE_DIRECTORY(./test TEST_CPP)
#ADD_EXECUTABLE(testHelloSqrt ${TEST_CPP})
#TARGET_LINK_LIBRARIES(testHelloSqrt hellosqrt)

#INCLUDE_DIRECTORIES(. )
#source directory
#AUX_SOURCE_DIRECTORY(${PROJECT_SOURCE_DIR}/core CORE_CPP_LIST)
#list(APPEND CPP_LIST ${CPP_LIST}  ${CORE_CPP_LIST})
#message(STATUS "cpplistcore =  ${CPP_LIST}")
#set(CORE_CPP_LIST ${CORE_CPP_LIST} PARENT_SCOPE)
#set extern libraries
#SET(EXT_LIB /usr/lib/x86_64-linux-gnu/libm.so)
