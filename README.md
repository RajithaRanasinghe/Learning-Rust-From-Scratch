# Learning Rust From Scratch

## Installing Rust on Linux or macOS
Open a terminal and enter the following command:

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

If you get linker errors, you should install a C compiler, which typically includes a linker. A C compiler is also useful because some common Rust packages depend on C code.

### Installing a C Compiler
- **macOS**: Run the following command to install Xcode tools, which includes a C compiler:
```sh
xcode-select --install
```
- **Linux**: Install **GCC** or **Clang** using your package manager (e.g., apt, dnf, or pacman).

## Installing Rust on Windows

On Windows, visit [Rust's official website](https://www.rust-lang.org/tools/install) and follow the installation instructions.

## Check Rust Installation

### Check Rust Version
Open **PowerShell** and run:
```sh
rustc --version

```
If Rust is installed and in the system **PATH**, this will display the installed Rust version.
### Check Cargo Version
Since **Cargo** (Rust's package manager) is installed alongside Rust, you can also check:
```sh
cargo --version


```


