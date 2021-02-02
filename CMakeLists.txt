cmake_minimum_required (VERSION 3.10)
project (cereal)

add_library(cereal INTERFACE)
target_include_directories(cereal SYSTEM INTERFACE
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
  $<INSTALL_INTERFACE:include>
)
