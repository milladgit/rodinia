# C compiler
CC = pgc++
CC_FLAGS = -acc -ta=tesla -Minfo=accel -O3 -std=c++11 -Mcuda

hotspot: 
	$(CC) $(CC_FLAGS) hotspot_openacc.cpp -o hotspot 

clean:
	rm -f hotspot
