# This repo contains an example for running Replica Exchange Solute Tempering 2 simulations in Frontier (OakRidge National Lab) using NAMD.

1. In this simulation, NMR data (in the form of dihedral restraints) are alos included. If they are not needed please comment out the extrabond part in trpv1-base.namd file.
2. If there are atom clash errors while using the NMR restraints, then run a separate MD simulation with just the restrains to obtain the corroesponding .coor and .xsc files with data. Then use them to start a REST2 simulation. In this case the user also needs to update the rest2-remd.namd file
3. 