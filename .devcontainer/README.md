# Dev Container Configuration

This folder contains the configuration for the development container for this C++ CMake project.

## What's Included

- **Base Image**: Microsoft's official C++ development container (Debian 12)
- **Build Tools**:
  - CMake (latest)
  - Ninja build system
  - GCC/G++ compiler toolchain
  - GDB debugger
- **Shell**: Zsh with Oh My Zsh
- **VS Code Extensions**:
  - C/C++ Extension Pack
  - CMake Tools
  - CMake language support
  - Better C++ Syntax
  - Makefile Tools

## Getting Started

1. Open this folder in VS Code
2. When prompted, click "Reopen in Container" (or use Command Palette: "Dev Containers: Reopen in Container")
3. Wait for the container to build and configure
4. Start developing!

## Building the Project

Once inside the container, you can build the project using:

```bash
# Configure with CMake preset
cmake --preset debug

# Build
cmake --build build/debug

# Run the executable
./build/debug/hello_world
```

Or use the CMake Tools extension from VS Code's command palette or status bar.

## Docker Socket Access

The container has access to the host's Docker socket, allowing you to build and test Docker images from within the dev container itself.
