#macro section
COM = g++
BIN = binary/
OBJ = object/
INC = include/
SRC = source/
CFLAG = -c
OFLAG = -o

all: build-server build-client

 
build-server: compile-func 
	${COM} ${OFLAG} ${BIN}server12 ${SRC}server.cpp ${OBJ}func.o
compile-func:
	${COM} ${CFLAG} ${OFLAG} ${OBJ}func.o ${SRC}func.cpp

build-client: 
	${COM} ${OFLAG} ${BIN}client12 ${SRC}client.cpp

ss:
	./${BIN}server12
sc:
	./${BIN}client12

clean:
	rm ${OBJ}func.o ${BIN}server12 ${BIN}client12


