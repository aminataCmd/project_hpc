CC=gcc -Wall -O3 -fopenmp -g

all: ec_omp ec_seq

ec_seq: exact_cover_seq.c
	$(CC) exact_cover_seq.c -o ec_seq
	./ec_seq --in ../Instances/bell12.ec
	./ec_seq --in ../Instances/bell13.ec
	./ec_seq --in ../Instances/bell14.ec

ec_omp: exact_cover_openmp.c																																																																																																											
	$(CC) exact_cover_openmp.c -o ec_omp
	./ec_omp --in ../Instances/bell12.ec
	./ec_omp --in ../Instances/bell13.ec
	./ec_omp --in ../Instances/bell14.ec

ec_omp2: exact_cover_openmp2.c
	$(CC) exact_cover_openmp2.c -o ec_omp2
	./ec_omp2 --in ../Instances/matching8.ec
	./ec_omp2 --in ../Instances/matching9.ec
	./ec_omp2 --in ../Instances/matching10.ec

ec_omp3: exact_cover_openmp3.c																																																																																																											
	$(CC) exact_cover_openmp3.c -o ec_omp3
	#./ec_omp3 --in ../Instances/matching8.ec
	#./ec_omp3 --in ../Instances/matching9.ec
	#./ec_omp3 --in ../Instances/matching10.ec
	./ec_omp3 --in ../Instances/matchin.ec

ec_mpi: exact_cover_mpi.c
	$(CC) exact_cover_mpi.c -o ec_mpi
	./ec_mpi --in ../Instances/matching9.ec


clean:
	rm -f exact_cover_seq.o exact_cover_openmp.o exact_cover_openmp2.o exact_cover_openmp3.o exact_cover_mpi.o  ec_seq ec_omp ec_omp2 ec_omp3 ec_mpi
