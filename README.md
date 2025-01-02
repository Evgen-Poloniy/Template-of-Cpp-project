# 1. Install make
Input this commands in terminal:

1.1. For Linux distributions

* Ubuntu/Debian 

```
sudo apt-get update | sudo apt install make
```

* Fedora:

```
sudo dnf install make
```

* CentOS/RHEL:

```
sudo yum install make
```

* Arch Linux:

```
sudo pacman -S base-devel

```

1.2. For MacOS:

```
xcode-select --install
```

1.3. For Windows

Use MSYS2 and input command in termainal:

```
pacman -S make
```

# 2. Create working dirеctories
2.1. Create directory, then go to this directoty:

```
cd <some directories>
```

2.2. Input this command in terminal to create "src", "headers" and build" directories and main.cpp file:

```
make create
```

2.3. If you want to create directories with **git** initialization, use this command:

```
make gcreate
```

* Be warned, this command performs commant **git init** and creates hidden folder with **git** configuration file

You may change name of this directories in Makefile (change points 7.1 - 10)

# 3. Compile your project
In Makefile you can choose some parametrs:

Type of build:

```
#-----------------------------------------|
# 1. Choose Debug/Release:                |
BUILD = Debug
#-----------------------------------------|
```

Bitness of architecture:

```
#-----------------------------------------|
# 2. Choose x32/x64:                      |
ARCH = x64
#-----------------------------------------|
```

Platform:

```
#-----------------------------------------|
# 3. Choose platforms Win/Linux/Mac       |
PLATFORM = Linux
#-----------------------------------------|
```

And differend parametrs by point 10 

Input this command in terminal to compile your project:

```
make comp
```

# 4. Run your project
Input this command in terminal:

```
make run
```

Also, you may compile and run project by command:

```
make all
```

# 5. Send your project to GitHub
Input this command in terminal:

```
make gpush
```

`
Enter the names of files and/or directories to send to GitHub:
`
as you do when using the **git init** command

`
Enter commit message
`
without ""

# 6. Clear directories with executable objective files
Input this command in terminal:

```
make clean
```
 
____

>Edit Makefile for your purpose