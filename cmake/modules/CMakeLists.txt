
set(DISPATCH_EXPORTS_FILE ${CMAKE_CURRENT_BINARY_DIR}/dispatchExports.cmake)
configure_file(dispatchConfig.cmake.in
  ${CMAKE_CURRENT_BINARY_DIR}/dispatchConfig.cmake)

get_property(DISPATCH_EXPORTS GLOBAL PROPERTY DISPATCH_EXPORTS)
export(TARGETS ${DISPATCH_EXPORTS} FILE ${DISPATCH_EXPORTS_FILE})
