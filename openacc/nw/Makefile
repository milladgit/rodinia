# C compiler
CC = pgc++
CC_FLAGS = -w -mp -acc -ta=tesla -Minfo=accel -O3 -std=c++11

needle: needle.cpp
	$(CC) $(CC_FLAGS) needle.cpp -o needle 

clean:
	rm -f needle 
