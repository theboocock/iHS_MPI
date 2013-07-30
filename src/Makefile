CC=g++
MPI_LINK=$(shell mpic++ --showme:link)
MPI_COMPILE_FLAGS=$(shell mpic++ --showme:compile)

CFLAGS=-c -Wall
LDFLAGS=
SOURCES=Ehh.cc PData.cc
OBJECTS=$(SOURCES:.cc=.o)
EXECUTABLE=ihs


all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
		$(CC) $(MPI_COMPILE_FLAGS) $(LDFLAGS) $(OBJECTS) $(MPI_LINK) -o $@
.cc.o:
		$(CC) $(CFLAGS) $(MPI_COMPILE_FLAGS) $(MPI_LINK) $< -o $@
clean:
	rm -Rf $(EXECUTABLE) $(OBJECTS) 





