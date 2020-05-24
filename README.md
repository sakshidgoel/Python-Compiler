# Python-Compiler
All phases of a compiler for Python Language have been implemented using C language. The constructs 'if-else' and 'while' have been handled.  
  
## Introduction
The **_proj.l_** lex file and **_proj1.y_** yacc file work together to **parse** the Python code in the **_inp.py_** file and **generate tokens** to output a **symbol table** and create an **abstract syntax tree** and hence, generate the **optimised intermediate code**. This optimised intermediate code is saved in the file **_IntermediateCode.txt_** which is then accessed in the **_TargetCodeGenerator.c_** file. This file converts this optimised intermediate code to the **target code** for a hypothetic machine model which will be discussed further.  
  
## Steps To Run
1) Install Flex (to make lex program work)
```
sudo apt-get upgrade
sudo apt-get install flex
```
2) Install Bison (to make yacc program work)
```
sudo apt-get upgrade
sudo apt-get install bison
```
3) Run the lex and yacc files
```
lex proj.l && yacc -d -v proj1.y && gcc lex.yy.c y.tab.c -ll -lm -w
```
4) Run the TargetCodeGenerator.c file
```
gcc -o TargetCodeGenerator .\TargetCodeGenerator.c
.\TargetCodeGenerator.exe
```  

## Implementation

### Context Free Grammar

### Parsing and Token Generation

### Symbol Table Creation

### Abstract Syntax Tree

### Intermediate Code Generation

### Code Optimization

### Error Handling

### Target Code Generation

## Snapshots of Sample Input and Output

## Contact
For any comments or questions, please email at sakshidgoel@gmail.com / amoghrajesh1999@gmail.com / tanvipk99@gmail.com
