# C compiler
CC = pgc++
CC_FLAGS = -mp -acc -ta=tesla -Minfo=accel -O3 -std=c++11 -Mcuda

# CC_FLAGS+=-g 

bfs: bfs.cpp
	$(CC) $(CC_FLAGS) bfs.cpp -o bfs 

clean:
	rm -f bfs result.txt
