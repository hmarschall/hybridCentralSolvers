# hybridCentralSolvers
United collection of hybrid  Central solvers - one-phase, two-phase and multicomponent versions.

Only OpenFOAM+ version of the OpenFOAM technology is supported sinces 2018. Use branches digitef-dev-YYMM, where YYMM - corresponds to OpenFOAM+ version, for example 1812

1. **pimpleCentralFoam** - Pressure-based semi implicit compressible flow of perfect gas solver based on 
central-upwind schemes of Kurganov and Tadmor with LTS support for steady-state calculations

2. **rhoPimpleCentralFoam** - Pressure-based semi implicit compressible flow  of real gas solver based on 
central-upwind schemes of Kurganov and Tadmor and LTS support for steady-state calculations

3. **pimpleCentralDyMFoam** - Pressure-based semi implicit compressible flow of perfect gas solver based 
on central-upwind schemes of Kurganov and Tadmor with mesh motion and LTS support for steady-state calculations

4. **reactingPimpleCentralFoam** - Pressure-based semi implicit compressible flow solver based on central-upwind schemes of 
Kurganov and Tadmor for combustion with chemical reactions and LTS support for steady-state calculations

5. **twoPhaseMixingCentralFoam** - Transient Eulerian two-phase solver. Liquid and gas are
    considered as compressible fluids. Mass transfer at the interface is not accounted.

6. **twoPhaseMixingCentralDyMFoam** - Transient Eulerian two-phase solver with dynamic meshes. Liquid and gas are
    considered as compressible fluids. Mass transfer at the interface is not accounted.

7. **chtMultiRegionCentralFoam** -     Pressure-based semi implicit solver, based on hybrid central-upwind schemes
    of Kurganov and Tadmor for conjugate simulation of compressible flows of perfect gas (Mach 
    number is ranging from 0 to 6) and solid body heat transfer.

Telegram public group: https://t.me/hybridCentralSolvers for questions and discussion of the solvers features

Available OpenFOAM versions:
* OpenFOAM 3.1 - master branch
* OpenFOAM 4.1 - dev-of4.1 branch
* OpenFOAM 6   - dev-of6 branch
* OpenFOAM+ 1812 - digitef-dev-1812
* OpenFOAM+ 1912 - digitef-dev-1912
* OpenFOAM+ 2012 - digitef-dev-2012

## The library was useful in next research studies.

### >>>>> 2021 <<<<<

| Title | Description |
|------|-------------|
|[Development of a new OpenFOAM solver using regularized gas dynamic equations](https://www.mdpi.com/2311-5521/6/8/274)| ![Jet with particles Logo](https://www.mdpi.com/fluids/fluids-06-00274/article_deploy/html/images/fluids-06-00274-ag-550.jpg) |

###  >>>>> 2019 <<<<<
| Title | Description |
|------|-------------|
|[Numerical method to simulate detonative combustion of hydrogen-air mixture in a containment](https://doi.org/10.1080/19942060.2019.1660219)| ![Containement](https://www.tandfonline.com/na101/home/literatum/publisher/tandf/journals/content/tcfm20/2019/tcfm20.v013.i01/19942060.2019.1660219/20191106/images/medium/tcfm_a_1660219_f0018_oc.jpg)|

###  >>>>> 2016 <<<<<
| Title | Description |
|------|-------------|
|[On the Stability of Supersonic Boundary Layers with Injection](https://thesis.library.caltech.edu/9755/)| ![Scheme of boundary layer interaction with jet](https://github.com/unicfdlab/hybridCentralSolvers/blob/master/boundary-layer.png)|

   When using these solvers, please cite the following works:
   * [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3878441.svg)](https://doi.org/10.5281/zenodo.3878441)
   * Kraposhin MV, Banholzer M, Pfitzner M, Marchevsky IK. A hybrid pressure‐based solver for nonideal single‐phase fluid flows at all speeds. Int J Numer Meth Fluids. 2018;88:79–99. https://doi.org/10.1002/fld.4512
   * Kraposhin MV, Strijhak SV, Bovtrikova A Adaptation of Kurganov-Tadmor Numerical Scheme for Applying in Combination with the PISO Method in Numerical Simulation of Flows in a Wide Range of Mach Numbers. Procedia Computer Science. 2015;66:43-52. https://doi.org/10.1016/j.procs.2015.11.007
