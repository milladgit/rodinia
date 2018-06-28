
LOCAL_CC = gcc -g -O3 -Wall
CC = pgc++
CFLAGS = -mp -acc -ta=tesla -Minfo=accel -O3 -std=c++11 


all : nn

clean :
	rm -rf *.o nn hurricane_gen

nn : nn_openacc.cpp
	$(CC) $(CFLAGS) -o $@ $< $(LDFLAGS) -lm 

hurricane_gen : hurricane_gen.c
	$(LOCAL_CC) -o $@ $< -lm

