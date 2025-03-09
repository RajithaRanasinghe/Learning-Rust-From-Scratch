# Learning Rust From Scratch

## Installing Rust on Linux or macOS
Open a terminal and enter the following command:

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

If you get linker errors, you should install a C compiler, which typically includes a linker. A C compiler is also useful because some common Rust packages depend on C code.

### Installing a C Compiler
- **macOS**: Run the following command to install Xcode tools, which includes a C compiler:
```
xcode-select --install
```
- **Linux**: Install **GCC** or **Clang** using your package manager (e.g., apt, dnf, or pacman).

## Installing Rust on Windows

On Windows, visit [Rust's official website](https://www.rust-lang.org/tools/install) and follow the installation instructions.

## Check Rust Installation

### Check Rust Version
Open **PowerShell** and run:
```powershell
rustc --version

```
If Rust is installed and in the system **PATH**, this will display the installed Rust version.
### Check Cargo Version
Since **Cargo** (Rust's package manager) is installed alongside Rust, you can also check:
```
cargo --version
```

## Writing Your First Rust Program
It’s traditional when learning a new language to write a program that prints **"Hello, world!"** to the screen. Let’s do that in Rust!

### Step 1: Create a Project Directory
You’ll start by creating a directory to store your Rust code. Open a terminal and run the following commands:
```
mkdir projects
cd .\projects\
mkdir hello_world
cd .\hello_world\
```

### Step 2: Create a Rust Source File
Create a new file called **main.rs** Rust files always end with the **.rs** extension. If your filename has multiple words, use underscores to separate them (e.g., **hello_world.rs**).

### Step 3: Write the "Hello, World!" Program
Open the **main.rs** file in your favorite text editor or IDE and add the following code:
```
fn main() {
    println!("Hello, world!");
}
```
Save the file after adding the code.

### Step 4: Compile and Run the Program
Now, go back to your terminal and run the following commands to compile and execute the program:

On Linux/macOS:
```
rustc main.rs
./main
```

On Windows (CMD):
```PS
rustc main.rs
.\main.exe
```
If everything works correctly, you’ll see **"Hello, world!"** printed on your screen. Congratulations! You’ve just written your first Rust program.

## Anatomy of the "Hello, World!" Program
Let’s break down the program step by step:

1. The **main** Function:
