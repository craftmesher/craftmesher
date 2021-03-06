# CRack And deFecT Mesher
The crack and defect mesher is a tool written in C++ that is able to generate gradated tetrahedral meshes of polycrystals informed by the cracks and defects in the model.

If you use this tool or its key elements in your publication, we kindly ask you cite the following publication:

```
B.R. Phung, J. He, A.D. Spear. "A surface-mesh gradation tool for generating gradated tetrahedral meshes of microstructures with defects" Computational Materials Science 197 (2021) 110622.
```

```
@article{PHUNG2021110622,
  title = {A surface-mesh gradation tool for generating gradated tetrahedral meshes of microstructures with defects},
  journal = {Computational Materials Science},
  volume = {197},
  pages = {110622},
  year = {2021},
  issn = {0927-0256},
  doi = {https://doi.org/10.1016/j.commatsci.2021.110622},
  url = {https://www.sciencedirect.com/science/article/pii/S0927025621003499},
  author = {Brian R. Phung and Junyan He and Ashley D. Spear},
  keywords = {Numerical simulation, Polycrystal, Finite element modeling, Short crack, Voids},
}
```

# INSTALL INSTRUCTIONS

## Prerequisites
* Boost
* Python
* TetGen

## Linux: autotools
```
aclocal  
autoconf  
automake --add-missing  
./configure  
make  
```

## macOS with Clang (Intel and AS)

### Compile and build boost libraries  
* Download https://www.boost.org/users/download/#live  
* Unpack the archive  
* cd into directory  
* ./bootstrap.sh --prefix=/some/directory/to/install/boost/to  
* ./b2  
* ./b2 install  

### Make
* Set boost inc and lib directories in Makefile_macOS  
* Rename Makefile_macOS to Makefile  
* Run make  

