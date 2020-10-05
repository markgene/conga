# the compiler
CC = g++

## compiler flags:

# debugging
#CCFLAGS  = -g -std=c++11 -Wall

# production
CCFLAGS  = -O3 -std=c++11 -Wall

# 
INCLUDES = -I ./include/

# recompile if any .hh files changed
HHS = ./src/*.hh

all: ./bin/find_neighbors ./bin/calc_distributions


./bin/find_neighbors:  ./src/find_neighbors.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ./bin/find_neighbors ./src/find_neighbors.cc

./bin/calc_distributions:  ./src/calc_distributions.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ./bin/calc_distributions ./src/calc_distributions.cc


clean:
	-rm ./bin/*