
CC = pgc++
SRC = pathfinder.cpp
EXE = pathfinder
FLAGS = -w -mp -acc -ta=tesla -Minfo=accel -O3 -std=c++11 

all: release

release:
	$(CC) $(SRC) $(FLAGS) -o $(EXE)

debug:
	$(CC) $(SRC) -g -Wall -o $(EXE)

clean:
	rm -f pathfinder out


