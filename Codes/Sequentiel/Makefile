CC=gcc -Wall -O3 -g

all: ec_seq 


ec_seq: exact_cover_seq.c																																																																																																											
	$(CC) exact_cover_seq.c -o exact_seq
	./ec_seq --in ../Instances/bell12.ec
	./ec_seq --in ../Instances/bell13.ec
	./ec_seq --in ../Instances/bell14.ec
	./ec_seq --in ../Instances/matching8.ec
	./ec_seq --in ../Instances/matching9.ec
	./ec_seq --in ../Instances/matching10.ec


clean:
	rm -f exact_cover_seq.o exact_seq
