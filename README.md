# LLGLCI
CI builds of LLGL for x86 platform

# How to use

See [cmake](cmake) folder for include files. Then in your own library `CMakeLists.txt` do:

```cmake
find_package(LLGL REQUIRED)

...

target_link_libraries(<libname>
  ...
  LLGL::LLGL
  LLGL::OPENGL
  LLGL::VULKAN
  LLGL::D3D11
  LLGL::D3D12
	...
)
```