# 
# Sample Makefile for project 1 (COMP30017)
#
# The program used for illustration purposes is
# a simple program using prime numbers
#


## CC  = Compiler.
## CFLAGS = Compiler flags.
CC	= gcc
CFLAGS 	= -Wall  


## OBJ = Object files.
## SRC = Source files.
## EXE = Executable name.

SRC =		server.c game.c linked_list.c
OBJ =		server.o game.o linked_list.o
EXE = 		server

## Top level target is executable.
$(EXE):	$(OBJ)
		$(CC) $(CFLAGS) -o $(EXE) $(OBJ) -lm


## Clean: Remove object files and core dump files.
clean:
		/bin/rm $(OBJ) 

## Clobber: Performs Clean and removes executable file.

clobber: clean
		/bin/rm $(EXE) 

## Dependencies

##driver.o:	prime.h
##prime.o:	prime.h

linked_list.o: linked_list.h
game.o: game.h
server.o: server.h