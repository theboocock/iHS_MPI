iHS_MPI
=======


Calculates iHS using the original code provided
by Voight et al.

The difference is that the code now uses MPI instead 
of the standard single core for loop.

program is run as follows.

- `mpirun -n 4 ./ihs <mapfile> <hapfile>`





Integrate haplotype score and iES calculated using OpenMPI.
