# Simple Lex Yacc Calculator

Run the following commands to generate the lexer and parser files (lex.yy.c, cal.tab.c, and cal.tab.h):


flex calc.l      # Generate lex.yy.c (the lexer source code)
Compiler Report (after running flex calc.l):


Flex scanner generates lex.yy.c

bison -d calc.y  # Generate calc.tab.c and cal.tab.h (the parser source code and header file)
Compiler Report (after running bison -d calc.y):

Bison parser generates cal.tab.c and cal.tab.h
Compile the Code:

Now, compile your lexer and parser code along with any additional code. Include the math library (-lm) since you're using math functions:


gcc -o calculator cal.tab.c lex.yy.c -lm
Compiler Report (after running gcc):


Compilation completed successfully
If there are any compilation errors or warnings, they will be displayed in the compiler report at this stage.

Run the Calculator:

After successful compilation, you can run your calculator using the following command:

./calculator
This will execute your calculator program, and you can start entering expressions or commands.

Each step above includes the respective compiler report, indicating the outcome of that step. Please ensure that you are in the same directory as your calc.l and calc.y files when you run these commands, or provide the correct file paths if they are in different directories.
 
