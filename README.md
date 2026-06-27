# KineticSync

KineticSync is a high-velocity networking framework plugin for the **CarnageEngine**. Engineered for high-intensity, physics-driven action, it provides low-latency state synchronization and robust packet management.

## Overview

KineticSync is designed to operate seamlessly within the CarnageEngine architecture. It leverages C++20 standard features to deliver high-performance networking capable of handling fast-paced entity interpolation, client-side prediction, and authoritative server reconciliation.

### Core Features
* **High-Velocity Synchronization:** Optimized for real-time physics state transmission.
* **CarnageEngine Integration:** Seamlessly modular; designed to be integrated as a plugin via CMake.
* **C++20 Architecture:** Utilizes modern C++ concepts and patterns for type-safe, performant network contracts.

## Integration

KineticSync is intended to be included as a submodule within the `Plugins/` directory of the CarnageEngine source tree.

### Build Requirements
* **Compiler:** C++20 compliant compiler (GCC 11+, Clang 13+, MSVC 19.29+).
* **Build System:** CMake 3.20 or higher.
* **Engine Dependency:** Requires access to CarnageEngine header files and internal build environment.

### Setup
1.  Navigate to your local `CarnageEngine` repository.
2.  Add as a submodule:
    ```bash
    git submodule add <repository-url> Plugins/KineticSync
    ```
3.  Include in your project's `CMakeLists.txt`:
    ```cmake
    add_subdirectory(Plugins/KineticSync)
    target_link_libraries(YourTarget PRIVATE KineticSync)
    ```

## Licensing

**KineticSync** is open-source software licensed under the **MIT License**. Feel free to use, modify, and contribute to this project. 

*Contributions are welcome! Please ensure all pull requests follow the engine's contribution guidelines.*
