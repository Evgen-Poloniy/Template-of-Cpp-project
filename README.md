# 1. Install make
Input command in terminal:

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

Use MSYS2 and input commande in termainal:

```
pacman -S make
```

# 2. Create working dirеctories
2.1. Create directory, then go to this directoty:

```
cd <somethink directories>
```

2.2. Input this commande in terminal to create "src", "headers" and build" directories and main.cpp file:

```
make create
```

You may change name of this directories in Makefile (change points 7.1 - 7.6)

# 3. Compile your project
Input this commande in terminal:

```
make comp
```

You can choose build type at point 1 and bitness of architecture at points 2
Also, you can change parametrs at points 1 - 7.6

# 4. Run your project
Input this commande in terminal:

```
make run
```

Also, you may compile and run project by commande:

```
make all
```

# 5. Clear directories with executable objective files
Input this commande in terminal:

```
make clean
```
 
____

>Edit Makefile for your purpose