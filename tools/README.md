# Build and Flash Tools

This directory contains helper scripts for building and flashing the AMP Platform Reference examples.

## build.sh

Wrapper script for building the project with CMake.

### Usage

```bash
./tools/build.sh [OPTIONS]
```

### Options

- `-p, --platform PLATFORM` - Target platform (generic, rp2350) [default: generic]
- `-t, --type TYPE` - Build type (Debug, Release) [default: Debug]
- `-b, --build-dir DIR` - Build directory [default: build]
- `-c, --clean` - Clean build directory before building
- `-h, --help` - Show help message

### Examples

```bash
# Build with defaults (generic, Debug)
./tools/build.sh

# Build for RP2350 in Release mode
./tools/build.sh -p rp2350 -t Release

# Clean and rebuild
./tools/build.sh --clean
```

## flash.sh

Script for flashing examples to RP2350 (Pico 2) board via USB.

### Usage

```bash
./tools/flash.sh [OPTIONS] EXAMPLE
```

### Arguments

- `EXAMPLE` - Example to flash (hello-amp, pingpong, shared-counter)

### Options

- `-b, --build-dir DIR` - Build directory [default: build]
- `-m, --mount MOUNT` - Mount point of Pico board (auto-detected if not specified)
- `-h, --help` - Show help message

### Examples

```bash
# Auto-detect mount point and flash
./tools/flash.sh hello-amp

# Specify mount point manually
./tools/flash.sh -m /media/RPI-RP2 pingpong
```

### Notes

1. Hold the BOOTSEL button while connecting the Pico 2 to enter bootloader mode
2. The board will appear as a USB mass storage device (RPI-RP2)
3. After flashing, the board will reboot automatically
4. Connect to the serial port (115200 baud) to see output

## Manual Build

If you prefer to build manually without the scripts:

```bash
# Configure
cmake -B build -DAMP_PLATFORM=generic

# Build all
cmake --build build

# Build specific target
cmake --build build --target hello-amp

# Install (optional)
cmake --install build --prefix /path/to/install
```

## Adding New Tools

To add new tools to this directory:

1. Create the script file (e.g., `tools/mytool.sh`)
2. Make it executable: `chmod +x tools/mytool.sh`
3. Add usage documentation in this README
4. Follow the existing script structure for consistency
