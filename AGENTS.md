# AGENTS

## Build from source

- Install prerequisites:
  - CMake
  - C/C++ compiler toolchain (e.g. `build-essential`)
  - Development files for libcurl (curl support is enabled by default)

  On Debian/Ubuntu:
  ```bash
  sudo apt-get update
  sudo apt-get install build-essential cmake libcurl4-openssl-dev
  ```

- Configure and build:
  ```bash
  cmake -B build
  cmake --build build --config Release
  ```
  Add `-j` to the build command for parallel compilation or pass `-DLLAMA_CURL=OFF` to disable curl.
