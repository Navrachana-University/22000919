# Project Title: Compiler for Surati Language

## Description:
This project implements a basic compiler for the Surati language using **Flex** and **Bison**.  
It supports:
- Lexical Analysis  
- Syntax Parsing  
- Intermediate Code Generation (Three-Address Code)

The compiler reads Surati source files and produces:
- `debug.txt`: Debugging outputs  
- `tac.txt`: Three-Address Code  

---

## Author:
**Prof. Vaibhavi Patel**  
**Name:** Abhay Shinde  
**Roll Number:** 22000919  

---

## How to Run:
### Option 1: Command Line Execution (Manual Steps)
1. **Run Flex to generate lexer:**
   ```bash
   flex lexer.l

2. **Run Bison to generate parser:**
    ```bash
   bison -d parser.y

3. **Compile the generated code**:
    ```bash
   gcc -o compiler.exe lex.yy.c parser.tab.c

4. **Execute**:
    ```bash
   type input1.txt | compiler.exe

### Option 2: Run via Jupyter Notebook

You can also run the compiler using the provided Jupyter Notebook (main.ipynb), which automates all the above steps using Python's subprocess module.

Ensure Python is installed and you are running the notebook in an environment with Flex, Bison, and GCC installed.

## Outputs:
- debug.txt: Debugging output
- tac.txt: Three address code

## Note:
Make sure you have Flex and Bison installed before running.

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/bPoO8GTw)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19517705&assignment_repo_type=AssignmentRepo)
