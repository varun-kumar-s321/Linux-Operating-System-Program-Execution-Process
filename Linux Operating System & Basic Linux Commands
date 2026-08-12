# **Linux Operating System & Basic Linux Commands**

## **📌 Overview**

This topic covers the fundamentals of the **Linux Operating System** and basic Linux commands required for **C programming and Embedded Systems development**.

The topic focuses on understanding the **Linux file system, terminal, file and directory management, paths, C program compilation, and the Vi/Vim text editor**.

---

## **🎯 Learning Objectives**

After completing this topic, I should be able to:

* **Understand the basic Linux Operating System structure.**
* **Understand the Linux file system hierarchy.**
* **Use the Linux terminal and command prompt.**
* **Navigate between directories.**
* **Create, copy, move, and delete files/directories.**
* **Understand absolute and relative paths.**
* **Compile C programs using GCC.**
* **Use the Vi/Vim editor to create and edit files.**
* **Perform basic Linux command-line operations.**

---

# **📚 Topics Covered**

## **1. Program Execution Process**

The basic process of executing a C program in Linux is:

### **Step 1: Write the Program**

First, write the C program using an editor such as **Vi/Vim**.

Example:

```c
#include <stdio.h>

int main()
{
    printf("Hello World\n");
    return 0;
}
```

### **Step 2: Save the Source File**

Save the program with a `.c` extension.

Example:

```text
program.c
```

### **Step 3: Compile the Program**

Use the **GCC compiler**:

```bash
gcc program.c
```

By default, GCC generates an executable file named:

```text
a.out
```

### **Step 4: Execute the Program**

Run the executable using:

```bash
./a.out
```

### **Complete Process**

```text
Write Program
     ↓
Save program.c
     ↓
Compile using GCC
     ↓
Generate executable
     ↓
Execute using ./a.out
```

---

# **2. Compiler**

A **compiler** is a software program that translates **high-level source code into machine-understandable code**.

## **Types of Compilers**

There are mainly two types:

1. **Native Compiler**
2. **Cross Compiler**

### **2.1 Native Compiler**

A **native compiler** is used when the **host system and target system are the same**.

```text
Host System = Target System
```

Example:

```text
Linux PC → Linux PC
```

### **2.2 Cross Compiler**

A **cross compiler** is used when the **host system and target system are different**.

```text
Host System ≠ Target System
```

Cross compilers are commonly used in **Embedded System development**.

Example:

```text
PC → ARM Microcontroller
```

---

# **3. Linux File System**

Linux uses a **hierarchical file system**.

The top-level directory is called the **root directory**, represented by:

```text
/
```

## **Important Linux Directories**

| **Directory** | **Description**                    |
| ------------- | ---------------------------------- |
| `/`           | **Root directory**                 |
| `/bin`        | **Essential Linux commands**       |
| `/boot`       | **Boot-related files**             |
| `/lib`        | **System libraries**               |
| `/etc`        | **System configuration files**     |
| `/home`       | **User home directories**          |
| `/proc`       | **Process and system information** |
| `/root`       | **Root user's home directory**     |
| `/tmp`        | **Temporary files**                |

### **Linux File System Structure**

```text
/
├── bin
├── boot
├── etc
├── home
├── lib
├── proc
├── root
└── tmp
```

---

# **4. Basic Linux Commands**

Linux commands are entered through the **terminal**.

---

## **4.1 Navigation Commands**

### **`pwd`**

Displays the **Present Working Directory**.

```bash
pwd
```

Example output:

```text
/home/user
```

---

### **`cd`**

Changes the current directory.

```bash
cd directory_name
```

Example:

```bash
cd Documents
```

---

### **`cd ..`**

Moves to the **parent directory**.

```bash
cd ..
```

Example:

```text
/home/user/Documents
        ↓
/home/user
```

---

### **`cd ~`**

Moves to the **user's home directory**.

```bash
cd ~
```

---

# **5. Listing Commands**

## **`ls`**

Lists files and directories.

```bash
ls
```

---

## **`ls -l`**

Displays detailed information about files and directories.

```bash
ls -l
```

It displays information such as:

* **File permissions**
* **Owner**
* **Group**
* **File size**
* **Date/time**
* **File name**

---

# **6. Directory Commands**

## **`mkdir`**

Creates a new directory.

```bash
mkdir directory_name
```

Example:

```bash
mkdir test
```

---

## **`rmdir`**

Removes an **empty directory**.

```bash
rmdir directory_name
```

Example:

```bash
rmdir test
```

---

## **`rm -r`**

Removes a directory and its contents **recursively**.

```bash
rm -r directory_name
```

Example:

```bash
rm -r test
```

**⚠️ Be careful with `rm -r` because it can delete files inside the directory.**

---

# **7. File Commands**

## **`cat`**

Displays the contents of a file.

```bash
cat filename
```

Example:

```bash
cat program.c
```

---

## **`cat >`**

Creates a new file or **overwrites an existing file**.

```bash
cat > file.txt
```

Enter the required text and press:

```text
Ctrl + D
```

to save and exit.

---

## **`cat >>`**

Appends new content to the end of an existing file.

```bash
cat >> file.txt
```

---

## **`cat -n`**

Displays file contents with **line numbers**.

```bash
cat -n file.txt
```

Example:

```text
1  Hello
2  Welcome
3  Linux
```

---

## **`more`**

Displays a large file **page by page**.

```bash
more filename
```

---

## **`less`**

Allows page-by-page viewing and navigation through a file.

```bash
less filename
```

---

# **8. File Manipulation Commands**

## **`cp`**

Copies a file from one location to another.

```bash
cp source destination
```

Example:

```bash
cp program.c backup.c
```

---

## **`cp -R`**

Copies a directory and its contents recursively.

```bash
cp -R source destination
```

Example:

```bash
cp -R project backup
```

---

## **`mv`**

Used to **move or rename** files and directories.

### **Rename a file**

```bash
mv old.c new.c
```

### **Move a file**

```bash
mv program.c Documents/
```

---

## **`rm`**

Removes a file.

```bash
rm filename
```

Example:

```bash
rm program.c
```

---

## **`clear`**

Clears the terminal screen.

```bash
clear
```

---

# **9. Absolute and Relative Paths**

Paths are used to specify the location of files and directories.

There are two important types:

1. **Absolute Path**
2. **Relative Path**

---

## **9.1 Absolute Path**

An **absolute path** starts from the **root directory `/`**.

Example:

```text
/home/user/test/file.c
```

It gives the complete location of the file from the root.

---

## **9.2 Relative Path**

A **relative path** is specified with respect to the **current working directory**.

Example:

```text
./test/file.c
```

Here:

```text
. → Current directory
.. → Parent directory
```

### **Difference**

```text
Absolute Path
      ↓
Starts from /

Relative Path
      ↓
Starts from current directory
```

---

# **10. Vi/Vim Editor**

**Vi/Vim** is a powerful text editor available in Linux.

It can be used to create and edit:

* **C source files**
* **Configuration files**
* **Text files**
* **Shell scripts**

---

## **10.1 Start Vi/Vim**

To open or create a C file:

```bash
vi filename.c
```

Example:

```bash
vi program.c
```

---

# **11. Vi/Vim Modes**

Vi/Vim mainly works using different modes.

## **11.1 Insert Mode**

**Insert Mode** is used to enter or modify text.

Common commands:

```text
i
a
o
O
```

### **`i`**

Insert text before the cursor.

### **`a`**

Append text after the cursor.

### **`o`**

Creates a new line below the current line and enters Insert Mode.

### **`O`**

Creates a new line above the current line and enters Insert Mode.

---

## **11.2 Command Mode**

Command Mode is used for:

* **Navigation**
* **Editing**
* **Searching**
* **Saving**
* **Exiting Vim**

Press:

```text
Esc
```

to return to Command Mode.

---

# **12. Save and Exit in Vi/Vim**

First press:

```text
Esc
```

Then use the required command.

## **`:w`**

Saves the file.

```text
:w
```

---

## **`:wq`**

Saves the file and quits.

```text
:wq
```

---

## **`:q!`**

Quits without saving changes.

```text
:q!
```

---

# **13. Important Vi/Vim Commands**

| **Command** | **Purpose**                   |
| ----------- | ----------------------------- |
| `i`         | **Insert text**               |
| `a`         | **Append text**               |
| `o`         | **New line below**            |
| `O`         | **New line above**            |
| `w`         | **Move to next word**         |
| `b`         | **Move to previous word**     |
| `yy`        | **Copy current line**         |
| `p`         | **Paste**                     |
| `dd`        | **Delete current line**       |
| `dw`        | **Delete word**               |
| `u`         | **Undo**                      |
| `/word`     | **Search for a word**         |
| `x`         | **Delete character**          |
| `G`         | **Move to last line**         |
| `0`         | **Move to beginning of line** |
| `:w`        | **Save file**                 |
| `:wq`       | **Save and quit**             |
| `:q!`       | **Quit without saving**       |

---

# **14. Complete Practical Workflow**

The following is a basic Linux workflow for C programming:

### **Step 1: Open Terminal**

```bash
Ctrl + Alt + T
```

### **Step 2: Check Current Directory**

```bash
pwd
```

### **Step 3: Create a Directory**

```bash
mkdir c_programs
```

### **Step 4: Enter the Directory**

```bash
cd c_programs
```

### **Step 5: Create/Open a C File**

```bash
vi program.c
```

### **Step 6: Enter Insert Mode**

Press:

```text
i
```

### **Step 7: Write the C Program**

```c
#include <stdio.h>

int main()
{
    printf("Hello World\n");
    return 0;
}
```

### **Step 8: Save and Exit**

Press:

```text
Esc
```

Then:

```text
:wq
```

### **Step 9: Compile the Program**

```bash
gcc program.c
```

### **Step 10: Execute the Program**

```bash
./a.out
```

### **Complete Flow**

```text
Terminal
   ↓
pwd
   ↓
mkdir c_programs
   ↓
cd c_programs
   ↓
vi program.c
   ↓
i → Write Program
   ↓
Esc
   ↓
:wq
   ↓
gcc program.c
   ↓
./a.out
   ↓
Output
```

---

# **15. Quick Revision**

### **Linux**

**Linux is an open-source operating system widely used for programming, servers, and embedded systems.**

### **Root Directory**

```text
/
```

### **Current Directory**

```bash
pwd
```

### **Change Directory**

```bash
cd
```

### **List Files**

```bash
ls
```

### **Create Directory**

```bash
mkdir
```

### **Remove Directory**

```bash
rmdir
```

### **Remove Directory Recursively**

```bash
rm -r
```

### **Copy**

```bash
cp
```

### **Move/Rename**

```bash
mv
```

### **Delete**

```bash
rm
```

### **Display File**

```bash
cat
```

### **Display Line Numbers**

```bash
cat -n
```

### **Open Vi**

```bash
vi filename.c
```

### **Compile C Program**

```bash
gcc program.c
```

### **Execute**

```bash
./a.out
```

---

## **👨‍💻 Author**

**Varun Kumar S**
