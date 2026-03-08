
```markdown
# 🛠️ Dolet Toolchain

The official binary distribution for the **Dolet** programming language compiler infrastructure. This repository provides the essential backend tools required to transform Dolet source code into high-performance executables.

## 📦 Version Information
To ensure full compatibility with the **Dolet Bootstrap** compiler and ecosystem, this toolchain includes:
* **LLVM/Clang/LLD**: `v21.1.8`
* **MLIR**: `v22.0.0git`
* **Target**: `x86_64-pc-windows-msvc`

## 📥 Downloads
The binaries are hosted as Release Assets to maintain a lightweight repository.
1. Navigate to the [Releases](https://github.com/dolet-lang/dolet-toolchain/releases) page.
2. Download the package: **`dolet-toolchain-v21.1.8-win64.zip`**.

## 🚀 Installation & Project Structure
For the **Dolet Compiler** to function correctly, you must place the binaries inside a `tools` directory at the **root** of your compiler project:

```text
Dolet-Compiler-Root/
├── tools/                <-- Place clang.exe, lld-link.exe, mlir-translate.exe here
├── src/
├── packages/
└── README.md

```

## 🛡️ Governance

* **Managed by**: `dolet-core` (Version control and updates).
* **Utilized by**: `ecosystem-devs` (Building GPU, Audio, and CV modules).

## ⚖️ License & Legal Notices

This toolchain distribution includes binaries from the **LLVM Project**.

* **LLVM/Clang/MLIR**: Licensed under the **Apache License v2.0 with LLVM Exceptions**.
* **Third-Party Software**: These binaries are provided "as is" without any warranties.

By using this toolchain, you agree to comply with the terms of the [LLVM License](https://llvm.org/LICENSE.txt). Dolet is an independent project and is not affiliated with the LLVM Foundation.

---

*Maintained by the [Dolet Organization*](https://www.google.com/search?q=https://github.com/dolet-lang)

