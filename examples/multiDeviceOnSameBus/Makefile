CXX=g++
CXXFLAGS=-I../../ -W -Wall
LDFLAGS=-lads1x15_tla2024 -L../../
EXEC=MultiDevice
SRC=multiDevice.cpp
OBJ=$(SRC:.cpp=.o)

all: $(EXEC)

$(EXEC): $(OBJ)
	$(CXX) -o $@ $^ $(LDFLAGS)

$(OBJ): $(SRC)
	$(CXX) -o $@ -c $< $(CXXFLAGS)

clean:
	rm -f $(OBJ)

mrproper: clean
	rm -f $(EXEC)
