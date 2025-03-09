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

## Writing Your First Rust Program
It’s traditional when learning a new language to write a program that prints **"Hello, world!"** to the screen. Let’s do that in Rust!

### Step 1: Create a Project Directory
You’ll start by creating a directory to store your Rust code. Open a terminal and run the following commands:
```sh
mkdir projects
cd .\projects\
mkdir hello_world
cd .\hello_world\
```

### Step 2: Create a Rust Source File
Create a new file called **main.rs** Rust files always end with the **.rs** extension. If your filename has multiple words, use underscores to separate them (e.g., **hello_world.rs**).

### Step 3: Write the "Hello, World!" Program
Open the **main.rs** file in your favorite text editor or IDE and add the following code:
```sh
fn main() {
    println!("Hello, world!");
}
```
Save the file after adding the code.

### Step 4: Compile and Run the Program
Now, go back to your terminal and run the following commands to compile and execute the program:

On Linux/macOS:
```sh
rustc main.rs
./main
```

On Windows (CMD):
```sh
rustc main.rs
.\main.exe
```
If everything works correctly, you’ll see **"Hello, world!"** printed on your screen. Congratulations! You’ve just written your first Rust program.

## Anatomy of the "Hello, World!" Program
Let’s break down the program step by step:

1. The **main** Function:
```sh
fn main() {
}
```
- The main function is the entry point of every Rust program. It’s where execution begins.

- The function is declared with **fn**, followed by the function name (**main**), parentheses **()**, and curly braces **{}**.

2. The **println!** Macro:
```sh
println!("Hello, world!");
```
- **println!** is a macro (not a function) that prints text to the screen.

- The **!** indicates that it’s a macro. Macros in Rust are powerful tools for code generation.

- The text **"Hello, world!"** is passed as an argument to the macro.

3. Semicolons:
- Most lines of Rust code end with a semicolon **;**, which indicates the end of an expression.

## Compiling and Running Are Separate Steps
In Rust, you must compile your program before running it. The **rustc** command compiles your code into an executable binary. For example:
```sh
rustc main.rs
```
This creates an executable file (**main** on Linux/macOS or **main.exe** on Windows). You can then run the executable:
```sh
./main
```
or on Windows
```sh
.\main.exe
```
This separation of compiling and running is different from interpreted languages like Python or JavaScript, where you can run code directly.

## Next Steps: Introducing Cargo
While **rustc** is great for simple programs, Rust’s built-in package manager and build tool, **Cargo**, is essential for managing larger projects. In the next section, we’ll explore how to use Cargo to create, build, and run Rust projects.