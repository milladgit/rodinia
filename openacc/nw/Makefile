# C compiler
CC = pgc++
CC_FLAGS = -w -acc -ta=tesla -Minfo=accel -O3 -std=c++11

needle: 
	$(CC) $(CC_FLAGS) needle.cpp -o needle 

clean:
	rm -f needle 
