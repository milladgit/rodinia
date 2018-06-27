# C compiler
CC = pgc++
CC_FLAGS = -w -acc -ta=tesla -Minfo=accel -O3 -std=c++11 

bfs: 
	$(CC) $(CC_FLAGS) srad.cpp -o srad 

clean:
	rm -f srad
