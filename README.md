# proton

Supporting information for: “Accelerated proton dissociation in excited state induces super-acidic microenvironment of graphene quantum dots”



Structures

The models of graphene oxide created in this work are found in the [model/structure_dft_opt](https://github.com/baowanc/proton/tree/main/model/structure_dft_opt) directory. As in the paper, 7 models of each type were created. For each model, we provide coordinates in an xyz file (in XYZ format).
The models were then hydrated by adding H2O molecules, the resulting models are found in the [model/structure_water](https://github.com/baowanc/proton/tree/main/model/structure_water) directory. 


Input files

ground_excited_opt_bader.gjf: Representative input file for Gaussian geometry optimization and bader charge calculation, for the model 6.

input_GQD_water_MD.inp: Representative input file for CP2K ab initio molecular dynamics, for the model 6 with water.


MD trajectories

The trajectories report the atomic positions at each time step, in XYZ format, visualized by vmd.
