all: DATE symbolicExecution.cpp
	clang++ -emit-llvm -c -g -o symbolicExecution.o symbolicExecution.cpp
	llvm-link -o symbolicExecutionDate.bc symbolicExecution.o date.o
DATE: ../date.h ../date.cpp
	clang++ -emit-llvm -c -g -o date.o ../date.cpp
