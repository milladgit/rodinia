# C compiler
CC = pgc++
CC_FLAGS = -w -mp -acc -ta=tesla -Minfo=accel -O3 -std=c++11 

hotspot: hotspot_openacc.cpp
	$(CC) $(CC_FLAGS) hotspot_openacc.cpp -o hotspot 

clean:
	rm -f hotspot
