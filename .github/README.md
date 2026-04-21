<!--
Keep this document short & concise,
linking to external resources instead of including content in-line.
See 'release/text/readme.html' for the end user read-me.
-->

# Blender

[![License](https://img.shields.io/github/license/blender/blender)](https://www.blender.org/about/license/)
[![Version](https://img.shields.io/github/v/release/blender/blender)](https://developer.blender.org/docs/release_notes/)
[![Build](https://img.shields.io/github/actions/workflow/status/blender/blender/build.yml?branch=main)](https://developer.blender.org/docs/handbook/building_blender/)

Blender is the free and open source 3D creation suite. It supports the entirety of the 3D pipeline—modeling, rigging, animation, simulation, rendering, compositing, motion tracking and video editing.

![Blender screenshot](https://code.blender.org/wp-content/uploads/2018/12/springrg.jpg "Blender screenshot")

## Quick Start

### Build from Source

Blender can be built on Linux, macOS, and Windows. For detailed instructions, see the [Building Blender](https://developer.blender.org/docs/handbook/building_blender/) handbook.

**Prerequisites:**
- CMake
- Python 3.11+
- Platform-specific build tools (Visual Studio on Windows, Xcode on macOS, GCC/Clang on Linux)

**Basic build:**
```bash
# Clone the repository
git clone https://github.com/blender/blender.git
cd blender

# Configure (Linux/macOS)
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build --parallel

# On Windows, use:
cmake -S . -B build -G "Visual Studio 17 2022" -A x64 -DCMAKE_BUILD_TYPE=Release
cmake --build build --parallel
```

The built executable will be at `build/bin/Release/blender` (or similar depending on platform).

## Project Pages

- [Website](https://www.blender.org) — Main project site
- [Reference Manual](https://docs.blender.org/manual/en/latest/index.html) — User documentation
- [Developer Documentation](https://developer.blender.org/docs/) — Building, contributing, API docs
- [Community](https://www.blender.org/community/) — Forums, Discord, Blender Cloud
- [Code Review & Bug Tracker](https://projects.blender.org) — Report issues and contribute code

## Contributing

Blender welcomes contributions! See the [Developer Documentation](https://developer.blender.org/docs/) for:
- [Building from source](https://developer.blender.org/docs/handbook/building_blender/)
- [Code style and conventions](https://developer.blender.org/docs/handbook/contributing/)
- [Submitting patches](https://developer.blender.org/docs/handbook/contributing/patches/)

## License

Blender as a whole is licensed under the **GNU General Public License, Version 3**. Individual files may have a different but compatible license.

See [blender.org/about/license](https://www.blender.org/about/license) for details.
