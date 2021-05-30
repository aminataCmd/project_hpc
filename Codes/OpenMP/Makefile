CC=gcc -Wall -O3 -fopenmp -g

all: ec_omp 


ec_omp: exact_cover_openmp.c																																																																																																											
	$(CC) exact_cover_openmp.c -o ec_omp
	./ec_omp --in ../Instances/bell12.ec
	./ec_omp --in ../Instances/bell13.ec
	./ec_omp --in ../Instances/bell14.ec


clean:
	rm -f exact_cover_seq.o exact_cover_openmp.o exact_cover_openmp2.o exact_cover_openmp3.o exact_cover_mpi.o  ec_seq ec_omp ec_omp2 ec_omp3 ec_mpi
