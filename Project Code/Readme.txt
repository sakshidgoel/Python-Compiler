Section: B

Project Title: Python Compiler (constructs: 'if-else', 'while') 
	       - Using C language till Optimisation of Intermediate Code.
	       - Using Python Language for Target Code Generation.

Team Members: Sakshi Goel(PES1201700148), Amogh Rajesh Desai(PES1201700180), Tanvi PK(PES1201700646)

Project Guide: Preet Kanwal

Project Abstract: All phases of a compiler for Python Language till intermediate code optimisation have been implemented using C language, while target code generation has been implemented using Python language. The constructs 'if-else' and 'while' have been handled. Syntax and Semantic Errors have been handled and panic mode recovery has been implemented in the lexer. Optimisation techniques used are constant propagation and packing temporaries.

Code Execution: 
1) The following commands can be used to execute the code in any of the folders except '5-Target_Code':
```
lex proj.l
yacc -d -v proj1.y
gcc lex.yy.c y.tab.c -ll -lm -w
./a.out
```
2) The following commands execute the code in the '5-Target_Code' folder:
```
python3 final.py
```

#############----- VARIOUS FOLDERS ------################
1) 1-Token_And Symbol_Table: This folder contains the code that outputs the tokens and the symbol table.
2) 2-Abstract_Syntax_Tree: This folder contains the code that displays the abstract syntax tree.
3) 3-Intermediate_Code_Generation: This folder contains the code that generates the symbol table before optimisations and the intermediate code.
4) 4-Optimised_ICG: This folder contains the code that generates the symbol table after optimisations, the quadruples table and the optimised intermediate code.
5) 5-Target_Code: This folder contains the code that displays the assembly code/target code.
6) Entire_Compiler: This folder contains the code that generates the all the above outputs at once and displays it on the terminal.

#############-----Building and Running the Code------#######
1) The following instructions are to be used to build and run the code in any of the folders except the '5-Target_Code' folder:
```
lex proj.l
yacc -d -v proj1.y
gcc lex.yy.c y.tab.c -ll -lm -w
./a.out
```

2) The following commands execute the code in the '5-Target_Code' folder:
```
python3 final.py
```