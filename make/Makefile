CXX = g++
CXXFLAGS = -std=c++11

SRC_FILES = $(wildcard *.cpp)
EXE_FILES = $(patsubst %.cpp,%,$(SRC_FILES))

all: $(EXE_FILES)

%: %.cpp
	$(CXX) $(CXXFLAGS) -o $@ $<

clean:
	rm -f $(EXE_FILES)

