

all: ec_omp ec_seq

ec_seq: exact_cover_seq.c
	gcc -Wall -O3 -fopenmp exact_cover_seq.c -o ec_seq
	./ec_seq --in ../Instances/matching9.ec

ec_omp: exact_cover_openmp.c
	gcc -Wall -O3 -fopenmp exact_cover_openmp.c -o ec_omp
	./ec_omp --in ../Instances/matching9.ec

ec_mpi: exact_cover_mpi.c
	gcc -Wall -O3 -fopenmp exact_cover_mpi.c -o ec_mpi
	./ec_mpi --in ../Instances/matching9.ec

clean:
	rm -f exact_cover_seq.o exact_cover_openmp.o exact_cover_mpi.o ec_seq ec_omp ec_mpi
