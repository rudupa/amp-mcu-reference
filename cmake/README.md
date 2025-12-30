# CMake Platform Configuration

This directory contains platform-specific CMake configuration files.

## Available Platforms

### generic (generic.cmake)

Default platform for building on host systems. This configuration allows the code structure to be built and tested on any system with a C compiler, though actual dual-core execution requires hardware support.

**Usage:**
```bash
cmake -B build -DAMP_PLATFORM=generic
```

### rp2350 (rp2350.cmake)

Configuration for the Raspberry Pi RP2350 dual-core ARM Cortex-M33 microcontroller.

**Usage:**
```bash
cmake -B build -DAMP_PLATFORM=rp2350
```

**Requirements:**
- ARM GCC toolchain (arm-none-eabi-gcc)
- Raspberry Pi Pico SDK (optional but recommended)

## Adding a New Platform

To add support for a new platform:

1. Create a new file: `cmake/platforms/myplatform.cmake`

2. Add platform-specific configuration:
   ```cmake
   message(STATUS "Using myplatform configuration")
   
   # Set compiler flags
   add_compile_options(-mcpu=cortex-m4 -mthumb)
   
   # Set linker scripts
   # set(LINKER_SCRIPT ${CMAKE_SOURCE_DIR}/path/to/linker.ld)
   
   # Add platform-specific definitions
   add_definitions(-DPLATFORM_MYPLATFORM)
   ```

3. Build with your platform:
   ```bash
   cmake -B build -DAMP_PLATFORM=myplatform
   cmake --build build
   ```

## Platform-Specific Overrides

Platform implementations can override weak symbols defined in the runtime:

- `amp_get_core_id()` - Get current core ID
- `amp_boot_core()` - Boot secondary core

See runtime source files for details on which functions can be overridden.
