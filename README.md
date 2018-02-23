# EMSL basis set library mirror

This repository is a mirror of the
[EMSL basis set library collection](https://bse.pnl.gov/bse/portal)
for quantum chemistry electronic structure calculations. The webpage
interface is nice to use, but sometimes the website has issues, hence
this repository. It is also nice having text files to work with rather
than an interface that requires a lot of mouse-clicking.

The Gaussian gbs files can be added to your Gaussian calculations
directly, without having to delete the atoms that are not in your
molecule. More directories (format for other software, conversion
tools, bibtex entries, etc.) will be added as I need them.

All credit goes to Dr. David Feller and the many contributors to the
EMSL basis set exchange. When publishing results obtained from use of
the Basis Set Exchange (BSE) software and the EMSL Basis Set Library,
please cite:

```
  The Role of Databases in Support of Computational Chemistry Calculations 
  Feller, D., J. Comp. Chem., 17(13), 1571-1586, 1996. 

  Basis Set Exchange: A Community Database for Computational Sciences 
  Schuchardt, K.L., Didier, B.T., Elsethagen, T., Sun, L.,
  Gurumoorthi, V., Chase, J., Li, J., and Windus, T.L.
  J. Chem. Inf. Model., 47(3), 1045-1052, 2007, doi:10.1021/ci600510j.
```

## Contents of the library

- `gbs/` : basis sets in Gaussian format. Use these files in Gaussian
  like this:
  ```
  # b3lyp gen
  [...]
  
  @mybasis.gbs/N
  
  ```
  or, if you have a pseudopotential to go with it, like this:
  ```
  # b3lyp genecp
  [...]
  
  @mybasis.gbs/N
  
  @mybasis.ecp/N
  
  ```
- `ecp/` : effective core potentials in Gaussian format.

- `info/` : information about the basis sets, including literature
  references.

