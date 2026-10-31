# Ghidra_Headless_Disassembler
Prerequisits :
An offifical ghidra release file (Already Included)

[Python 3.10](https://www.python.org/downloads/) or later.

Install [JDK 25 64bit](https://adoptium.net/en-GB/temurin/releases),

Quick Prerequisit Install:
sudo apt update
sudo apt install -y python3 python3-pip default-jdk


Usage:
The program by default will disassemble all files in a folder into an output folder.
"python disassemble.py" defaults to input folder being "ToDisassemble", output folder "Disassembled".

"python disassemble.py --input InputFolderPath" It can be used to disassemble the files in a specific folder by substituting said folders path into InputFolderPath, it takes both relative and absolute paths. Its output will still go into Disassembled.

"python disassemble.py --output OutputFolderPath" By specifying the file path to a desired output folder, the program will disassemble all files in ToDisassemble folder into the specified output folder.

"python disassemble.py --input InputFolderPath --output OutputFolderPath" It is also possible to define both input and output folders.

Limitations:
The program does not check whether a file to be disassembled is already present in the output folder, it will complete the disassembly and then replace the file already present in the output folder. If the goal is to disassemble in multiple batches its necessary to create multiple input folders and one output folder for best results.