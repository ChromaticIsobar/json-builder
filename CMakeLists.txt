project(json-builder)

add_library(jsonbuilder json-builder.c)
target_link_libraries(jsonbuilder jsonparser)
target_include_directories(jsonbuilder INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

install (TARGETS jsonbuilder DESTINATION lib)
install (FILES json-builder.h DESTINATION include)
