# SIAM LA electronic structure minitutorial

This repository contains the material for the minitutorial
*Linear algebra challenges in electronic structure simulations*
by Eric Cancès, Michael F. Herbst and Antoine Levitt,
which will be presented at SIAM LA on 13.05.2024.

It is a downsized version of the lecture material of
the [DFTK school 2022](https://school2022.dftk.org/).

## Presentations
- [Eric Cancès: Introduction to Density-Functional Theory](1_Eric_Cances.pdf)
- [Antoine Levitt: Density-Functional Theory: Algorithm](2_Antoine_Levitt.pdf)
- [DFTK tour and eigensolvers](3_eigensolvers.ipynb)
- [Self-consistent field methods](4_self_consistent_field.ipynb)
- [Analysing SCF convergence](5_analysing_scf_convergence.ipynb)

## Further reading
- [DFTK documentation](https://docs.dftk.org), in particular:
  * [Background on periodic problems and plane-wave discretisations](https://docs.dftk.org/dev/guide/introductory_resources/)
  * [Comparing discretization techniques](https://docs.dftk.org/dev/guide/discretisation/#Comparing-discretization-techniques)
  * [Introduction to DFT](https://docs.dftk.org/dev/guide/density_functional_theory/)
  * [Self-consistent field methods](https://docs.dftk.org/dev/guide/self_consistent_field/)
- [List of introductory resources](https://docs.dftk.org/dev/guide/introductory_resources/)

## Software and material
What you need to work with this material:

- [Julia 1.10](https://julialang.org/downloads/)
- [Jupyter](https://jupyter.org/) and [IJulia.jl](https://github.com/JuliaLang/IJulia.jl)
- This repository of workshop materials
- All required dependencies (Julia packages) for the workshop

### Getting Julia
For following the course you will need at least **Julia 1.10**.
Julia can be easily obtained in binary form from [Julia downloads](https://julialang.org/downloads/).

### Getting all the rest
To get the remaining files and dependencies
start up `julia` and in the resulting REPL shell,
copy and paste the following:

```julia
import Downloads
script = Downloads.download("https://raw.githubusercontent.com/mfherbst/2024-siamla-minitutorial/master/install.jl")
include(script)
```

This [downloads the install.jl script](https://raw.githubusercontent.com/mfherbst/2024-siamla-minitutorial/master/install.jl)
and runs it from julia.
Follow the instructions on the screen and start the Jupyter notebook server
with the command that will be printed.

As an alternative you can also also run the following commands manually
(this requires to have `git` and `julia` available from the commandline):
```
git clone https://github.com/mfherbst/2024-siamla-minitutorial
cd 2024-siamla-minitutorial
julia install-manual.jl
```

### Troubleshooting
If you are facing issues, check out
the [great troubleshooting section](https://carstenbauer.github.io/WorkshopWizard.jl/dev/troubleshooting/)
from the WorkshopWizard package by Carsten Bauer (which `install.jl` is using).

## Working with these notes online (Beta)
Click on the [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mfherbst/2024-siamla-minitutorial/master)
badge to work with these notes online (without a local Julia installation).
Note that for some of the exercises the computational performance available on
binder might not be sufficient.
