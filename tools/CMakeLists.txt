# =================================
# fastahack
#
# fastahack/CMakeLists.txt
# =================================

# set header and source files
set(FASTAHACK_TOOLS_SOURCES
	FastaHack.cpp
)

INCLUDE_DIRECTORIES(${FASTAHACK_SRC_INCLUDE})
#link_directories(${FASTAHACK_SRC_LIB_DIR})

#create binary
add_executable(fastahack
  ${FASTAHACK_TOOLS_SOURCES}
)

# link libraries to executables
target_link_libraries(fastahack
  ${FASTAHACK_SRC_LIB}
)
