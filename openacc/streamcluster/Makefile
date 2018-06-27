# include ../../common/make.config

CC = pgc++
CC_FLAGS = -w -acc -ta=tesla -Minfo=accel -O3 -std=c++11 


all: streamcluster

streamcluster: streamcluster.cpp streamcluster_kernel.cpp
	$(CC) $(CC_FLAGS) streamcluster.cpp streamcluster_kernel.cpp -o streamcluster 
	

clean:
	rm -f *.o *~ *.txt streamcluster
	
