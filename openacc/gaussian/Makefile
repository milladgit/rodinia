include ../../common/make.config

CC := pgc++
CCFLAGS := -acc -ta=tesla -Minfo=accel -O3 -std=c++11 -Mcuda

SRC = gaussian.c
EXE = gaussian

release: $(SRC)
	$(CC) $(CCFLAGS) $(SRC) -o $(EXE)

clean:
	rm gaussian
