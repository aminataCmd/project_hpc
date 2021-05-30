MPI=mpicc
MPIEX = mpiexec
CCFLAGS= -Wall -Wextra
OPTION = —-in 
INSTANCES = ../../Instances/


OBJ= $(SRC:.c=.o)
EXEC= exact_cover_mpi.c


all: ec_mpi 


ec_mpi: exact_cover_mpi.c
	$(MPI) $(CCFLAGS) exact_cover_mpi.c -o exact_mpi
	$(MPIEX) ec_mpi --in ../../Instances/bell12.ec
	$(MPIEX) ec_mpi --in ../../Instances/bell13.ec
	$(MPIEX) ec_mpi --in ../../Instances/bell14.ec

ec_mpi2: exact_cover_mpi.c
	$(MPI) $(CCFLAGS) exact_cover_mpi.c -o exact_mpi2
	$(MPIEX) ec_mpi2 --in ../../Instances/matching8.ec
	$(MPIEX) ec_mpi2 --in ../../Instances/matching9.ec
	$(MPIEX) ec_mpi2 --in ../../Instances/matching10.ec


clean : 
	rm -f exact_cover_mpi.o exact_mpi exact_mpi2 
	rm -f exact_cover_mpi.o ec_mpi