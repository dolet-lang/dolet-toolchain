
# 🛠️ Dolet Toolchain

The official pre-built binary distribution for the **Dolet** programming language compiler infrastructure. This repository provides the essential backend tools required to transform Dolet source code into high-performance executables.

## 📦 Core Components

This toolchain includes the specific versions of LLVM and MLIR binaries synchronized with the **Dolet Bootstrap** compiler:

* **`mlir-translate.exe`**: Responsible for converting Dolet's intermediate representation (MLIR) into LLVM IR.
* **`clang.exe`**: Acts as the primary backend for machine code generation and C/C++ interoperability.
* **`lld-link.exe`**: A high-performance linker used to produce final Windows executables (`.exe`).

## 🚀 Getting Started

### 1. Installation

To ensure consistency across the **dolet-core** and **ecosystem-devs** teams, please clone this repository into your local development environment:

```bash
git clone https://github.com/dolet-lang/dolet-toolchain.git

```

### 2. Environment Setup

Add the `bin` folder path to your system's **PATH** environment variable to allow the `dolet-bootstrap` compiler to invoke these tools globally.

## 🛡️ Governance

This repository is managed under the following structure:

* **Parent Team**: `dolet-core` (Responsible for versioning and toolchain updates).
* **Support Team**: `ecosystem-devs` (Utilizes the toolchain for building GPU, Audio, and CV modules).

## ⚠️ Version Consistency

All contributors must use the binaries provided in this repository. Using external or mismatched versions of MLIR/LLVM may lead to incompatible IR generation or linking errors during the build process.
