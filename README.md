# Computational chemistry - how to get started

This document has resources for people new to computational quantum chemistry. Mainly directed for people starting at [our lab](https://blogs.helsinki.fi/johansson-group/).

This list is currently quite rough looking, I'm constantly making updates :)


List of abbreviations:
  * DFT - Density functional theory
  * QC - Quantum chemistry
  * QM - Quantum mechanics
  * MD - Molecular dynamics

# Books and lecture notes

# Working with remote clusters

# Used methods

## Quantum chemistry

$H\Psi = E\Psi$

* Basis sets
* BO approximation
* HF
* Electron correlation
* DFT
  * Functionals

## Molecular dynamics
* Classical simulations
    * Potential is defined as a sum of bond, angle, dihedral, van der Waals, electrostatic terms
      * Parameters from experiments, QC calculations
  * No quantum mechanical effects
    * Bond breaking, polarization, ...

* Not very useful in our stuff, we mostly look at small molecules


# Software


## Quantum chemistry

* [ORCA](https://orcaforum.cec.mpg.de/)
  * [On CSC](https://research.csc.fi/software-details/-/asset_publisher/bwNv9EAV4eYX/content/orca)

* [Turbomole](http://www.turbomole.com/)
  * [On CSC](https://research.csc.fi/-/turbomole?redirect=https%3A%2F%2Fresearch.csc.fi%2Fsoftware%3Fp_p_id%3D101_INSTANCE_wfvLxzjnZlJx%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26p_p_col_id%3Dcolumn-2%26p_p_col_pos%3D1%26p_p_col_count%3D4%26p_r_p_564233524_categoryId%3D61753%26p_r_p_564233524_resetCur%3Dtrue)

* [Gaussian](http://gaussian.com/)
  * [On CSC](https://research.csc.fi/software-details/-/asset_publisher/bwNv9EAV4eYX/content/gaussian)

* [NWChem](http://www.nwchem-sw.org/index.php/Main_Page)
  * [On CSC](https://research.csc.fi/software-details/-/asset_publisher/bwNv9EAV4eYX/content/nwchem?redirect=https%3A%2F%2Fresearch.csc.fi%2Fsoftware-details%3Fp_p_id%3D101_INSTANCE_bwNv9EAV4eYX%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26p_p_col_id%3Dcolumn-2%26p_p_col_count%3D1)


## Molecular dynamics simulations

* [GROMACS](http://www.gromacs.org/)

## Visualization
* [Avogadro](https://avogadro.cc/)
  * Open source, quite powerful
  * Best tool for building molecules, UFF force field for preoptimization
  * Conformation search
  * Visualization of orbitals, vibrations, Bader analysis, ...
* [VMD](http://www.ks.uiuc.edu/Research/vmd/)
  * Excellent and scriptable program, heavily used in MD field

* [Chemcraft](https://www.chemcraftprog.com/)
  * Good for many manipulations, visualization
  * Not free, 150 days free trial period


## Scripting and working with data

### Python
  * Best choice!
  * Rich and modern environment
  * Excellent data science stack, useful libraries:
    * Numpy: linear algebra calculations and much more
    * SciPy: special functions, integrals, a lot of numerical tools
    * Matplotlib: plotting, excellent for visualizations
    * Pandas: "excel", data structures, good for data manipulation, analysis
    * Scikit-learn: Machine learning, regression, statistics
    * Keras, tensorflow: Deep learning, probably not needed yet

  * Jupyter Notebooks
    * Nice graphical user interface

### Bash tools
  * sed
  * awk
  * gnuplot

### [Cheminformatics](https://en.wikipedia.org/wiki/Cheminformatics)
* "Information technologies for chemistry"
#### Software
  * [RDKit](http://www.rdkit.org/docs/GettingStartedInPython.html)
    * Very nice open-source library, python interface
  * [CDK](https://cdk.github.io/)
    * Apparently quite good, in Java
#### Data structures for molecules
  * For storing, searching, ... [SMILES](https://en.wikipedia.org/wiki/Simplified_molecular-input_line-entry_system)
  * [SMARTS](https://en.wikipedia.org/wiki/Smiles_arbitrary_target_specification)
  * [InCHL](https://en.wikipedia.org/wiki/International_Chemical_Identifier)

#### Databases
  * Relational databases (MySQL, sqlite, postgreSQL, ...)
  * Non-relational (MongoDB, ...)
  * Pandas is quite good in my opinion
