CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(json_spirit)
INCLUDE_DIRECTORIES(json_spirit)
ADD_SUBDIRECTORY(json_spirit)
ADD_SUBDIRECTORY(json_demo)
ADD_SUBDIRECTORY(json_headers_only_demo)
ADD_SUBDIRECTORY(json_map_demo)
ADD_SUBDIRECTORY(json_test)

INSTALL(
  FILES
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_error_position.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_reader.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_reader_template.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_stream_reader.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_utils.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_value.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_writer.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_writer_template.h
  ${CMAKE_SOURCE_DIR}/json_spirit/json_spirit_writer_options.h
  DESTINATION include/json_spirit)

INCLUDE(CPack)
