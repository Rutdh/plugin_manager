cmake_minimum_required(VERSION 3.14.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(pstdata_parser)

set(SRCS
  main.cpp

)

add_executable(${PROJECT_NAME}
  ${SRCS}
)

CTPRD-20251022-000001265-99

target_include_directories(${PROJECT_NAME}
  PRIVATE
  ${CMAKE_CURRENT_SOURCE_DIR}/../risk_cms/src/sharedobj/CommonFactors
)
