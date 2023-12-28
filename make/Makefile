CC = gcc
CXX = g++
CFLAGS = -std=c11
CXXFLAGS = -std=c++11

SRC_FILES = $(wildcard *.c *.cpp)
EXE_FILES = $(patsubst %.c,%,$(filter %.c,$(SRC_FILES))) $(patsubst %.cpp,%,$(filter %.cpp,$(SRC_FILES)))

all: $(EXE_FILES)

%: %.c
	$(CC) $(CFLAGS) -o $@ $<

%: %.cpp
	$(CXX) $(CXXFLAGS) -o $@ $<

clean:
	rm -f $(EXE_FILES)
