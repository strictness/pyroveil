add_library(layer-util STATIC dispatch_helper.cpp dispatch_helper.hpp dispatch_wrapper.hpp)
target_include_directories(layer-util PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(layer-util PUBLIC Vulkan-Headers)
target_compile_options(layer-util PRIVATE ${PYROVEIL_CXX_FLAGS})
