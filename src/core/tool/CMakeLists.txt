set(tool_headers
  codegen_cmd.h
  index_cmd.h
  train_cmd.h
)

set(tool_sources
  codegen_cmd.cc
  index_cmd.cc
  jumanpp_tool.cc
  train_cmd.cc
)

add_executable(jumanpp_tool ${tool_sources} ${tool_headers})
target_link_libraries(jumanpp_tool jpp_core_train jpp_core_codegen)