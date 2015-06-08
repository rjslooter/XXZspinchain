# XXZspinchain
Quantum spin chain Hamiltonian in presence of magnetic field

The various functions that are included are used to calculate the eigenvalues of the Hamiltonian op a quantum spin chain (QSC). 
The calculated eigenvalues of the Hamiltonian operator represent energy values.
We allow for a magnetic field to work on the QSC, and we are interested in the lowest eigenvalues of the system. Some additional
function allows us to use a small orthogonal basis constructed out of the known eigenvectors at two specified points. From this
basis it is possible to approximate the real eigenvalues, but a lot faster.

Running the code for long chains, say more than 17 atoms, WILL take a long time, especially if one wants to know the eigenvalues
at a lot of steps of the magneticfield. 
e.g. Calculating 10 eigenvalues at 250 steps of the magnetic field strength for a 19 atoms chain can take several hours!

A DMRG method module has been included, the main part of this code has been copied from <https://github.com/simple-dmrg/simple-dmrg/>. Here we added the feature to activate a magnetic field. Al the credits for the rest of the program go to the original writers James R. Garrison and Ryan V. Mishmash.

Also a multiprocessing module and two functions to build Hamiltonian matrices for (next-)next-nearest neighbour interactions are included.
