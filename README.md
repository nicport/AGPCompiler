## Files needed
- lexer.l - the rules for AGP scanning. Contains an include to parser.tab.h.
- parser.y  - the rules AGP parsing
- symbol_table.c  
- tb_symbol_table.c
- example_agp - example code to give to the AGP compiler

## To build and run
To run the current version of the Asynchronous Graphical Compiler:
$ make
$ ./agc example_agp

------------------------------------------------------------------
This version correctly identifies tokens and checks the syntax of 
the input agp code. symtab_dump.out and revisit_dump.out are 
created once ./agc is ran. They contain all the identifiers in the 
symbol table and all subgraphs respectively