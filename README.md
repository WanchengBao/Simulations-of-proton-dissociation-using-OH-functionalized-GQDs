# Simulations-of-proton-dissociation-using-OH-functionalized-GQDs

Supporting information for: “Accelerated proton dissociation in excited state induces super-acidic microenvironment of graphene quantum dots”


**Structures**

The models of graphene oxide created in this work are found in the [model/structure_dft_opt](https://github.com/baowanc/proton/tree/main/model/structure_dft_opt) directory. As in the paper, 7 models of each type were created. For each model, we provide coordinates in an xyz file (in XYZ format).

The models were then hydrated by adding H2O molecules, the resulting models are found in the [model/structure_water](https://github.com/baowanc/proton/tree/main/model/structure_water) directory. 


**Input files**

ground_excited_opt_bader.gjf: Representative input file for [Gaussian](https://gaussian.com/gaussian16/) geometry optimization for the model 6.

input_GQD_water_MD.inp: Representative input file for [CP2K](https://www.cp2k.org/) ab initio molecular dynamics, for the model 6 with water.


**MD trajectories**

The trajectories report the atomic positions at each time step, in XYZ format, visualized by [vmd](https://www.ks.uiuc.edu/Research/vmd/).

The bader charge calculation performed by [bader](https://theory.cm.utexas.edu/henkelman/code/bader/)


#################################################### System Requirements ########################################################

The software performs well on any Linux Distribution. It was tested in OpenSuse and Centos frameworks. Windows users are recommended using a virtual emulation of Linux, for example any version of Ubuntu.

Running time may vary between minutes and days depending on the problem to be solved. 

Note: Some programs were only testet on large supercomputers and might consume too much memory for your device.


################################################### General Code structure ######################################################

Input:

- The aimd codes can read a topology file containing information about particle position.

Output: 

- System configurations in a .xyz format (for vmd)
- charge distributions in a ACF.dat format (for bader charge)
 
