# CUDA_SDK_PATH = /af10/sc5nf/NVIDIA_CUDA_SDK

OMP_NUM_THREADS = 16
ITERATIONS=1

CC = pgc++
CC_FLAGS = -w -mp -acc -ta=tesla -Minfo=accel -O3 -std=c++11 

all: euler3d_cpu euler3d_cpu_double pre_euler3d_cpu pre_euler3d_cpu_double

euler3d_cpu: euler3d_cpu.cpp
	$(CC) $(CC_FLAGS) -Diterations=$(ITERATIONS) -Dblock_length=$(OMP_NUM_THREADS) euler3d_cpu.cpp -o euler3d_cpu
euler3d_cpu_double: euler3d_cpu_double.cpp
	$(CC) $(CC_FLAGS) -Diterations=$(ITERATIONS) -Dblock_length=$(OMP_NUM_THREADS) euler3d_cpu_double.cpp -o euler3d_cpu_double

pre_euler3d_cpu: pre_euler3d_cpu.cpp
	$(CC) $(CC_FLAGS) -Diterations=$(ITERATIONS) -Dblock_length=$(OMP_NUM_THREADS) pre_euler3d_cpu.cpp -o pre_euler3d_cpu

pre_euler3d_cpu_double: pre_euler3d_cpu_double.cpp
	$(CC) $(CC_FLAGS) -Diterations=$(ITERATIONS) -Dblock_length=$(OMP_NUM_THREADS) pre_euler3d_cpu_double.cpp -o pre_euler3d_cpu_double


clean:
	rm -f euler3d_cpu
	rm -f euler3d_cpu_double
	rm -f pre_euler3d_cpu
	rm -f pre_euler3d_cpu_double
