C = gcc
CFLAGS += -pedantic-errors
CFLAGS += -Wall
CFLAGS += -g
CFLAGS += -lstdc++
.PHONY = clean


OBJS_1 = client_student.o 

SRCS_1 = client_student.c

HEADERS_1 = Student.h

EXECUTABLE = prog_2

#target: (the target of the make command) dependencies (files required to build target)
#	rule to build target (ISO compiler, Flags)


all: ${EXECUTABLE}

${EXECUTABLE}: ${HEADERS_1} ${OBJS_1}
	${C} ${CFLAGS} ${OBJS_1} -o ${EXECUTABLE}

${OBJS_1}: ${SRCS_1}
	${C} ${CFLAGS} -c ${@:.o=.c}

clean:
	rm -rf *o *~ ${EXECUTABLE}
