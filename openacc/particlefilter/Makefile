#makefile

CC = pgcc
FLAGS = -w -acc -ta=tesla -Minfo=accel -O3 

all: ex_particle_OPENACC_seq.c
	$(CC) $(FLAGS) ex_particle_OPENACC_seq.c -o particle_filter -lm

# openmp: ex_particle_OPENACC_seq.c
# 	$(CC) -O3 $(FLAGS) ex_particle_OPENACC_seq.c -o particle_filter -lm
	

clean:
	rm -rf *.o particle_filter
