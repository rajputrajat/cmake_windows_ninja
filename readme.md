# Using Cmake on Windows (crossplatform) without relying on MSVS - using Ninja and clang toolchain

## How to use

### make sure you have ninja, cmake and llvm installed

```powershell
choco install ninja cmake llvm -y # using chocolatey
```

### add CC and CXX env (nushell examples)

```powershell
let-env CC = "clang"
let-env CXX = "clang++"
```

### initialize using ninja generator

```powershell
cmake -S ./ -B ./build -G "Ninja" # or 
```

### build

```powershell
cmake --build ./build --config Release
```

## reference

[link](https://stackoverflow.com/a/61449746/3964354)
