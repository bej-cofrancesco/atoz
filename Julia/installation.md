# Julia Installation Guide

## Required Software

- **Julia**: The Julia programming language (https://julialang.org/downloads/)
- **VS Code**: With Julia extension (recommended)
- **Jupyter Notebook**: For interactive development
- **Juno**: Julia IDE (alternative option)
- **Git**: For package management and version control

## File Extensions

- `.jl` - Julia source code files
- `.ipynb` - Jupyter notebooks with Julia kernel
- `.toml` - Project and manifest files (Project.toml, Manifest.toml)
- `.jmd` - Julia Markdown files
- `.jls` - Serialized Julia data
- `.jlso` - Julia serialized objects
- `.ji` - Julia precompiled header files
- `.dylib`, `.so`, `.dll` - Julia dynamic libraries (platform-dependent)
- `.jll` - BinaryBuilder.jl wrapper packages
- `.mem` - Memory dump files

## Package Management

```bash
# Open the Julia REPL
julia

# Enter package mode by pressing ]
# Then use these commands:

# Add a package
add PackageName

# Remove a package
rm PackageName

# Update packages
update

# Check status of packages
status

# Activate a specific project environment
activate ./path/to/project

# Create a new project
generate ProjectName

# Preview operations without making changes
preview add PackageName

# Pin a package to a specific version
pin PackageName@1.2.3

# Exit package mode by pressing backspace
```

## Running Julia Programs

```bash
# Run a Julia file
julia path/to/file.jl

# Run with specific number of threads
julia --threads=4 path/to/file.jl

# Run with optimizations
julia -O3 path/to/file.jl

# Run with math optimization mode
julia --math-mode=fast path/to/file.jl

# Run in interactive mode
julia -i path/to/file.jl

# Run code from command line
julia -e 'println("Hello, world!")'

# Start Julia REPL
julia

# Start Julia with a specific project environment
julia --project=path/to/project
```

## Common Libraries

- **Data Science**: DataFrames.jl, CSV.jl, Query.jl
- **Statistics**: Statistics.jl, StatsBase.jl, Distributions.jl
- **Machine Learning**: Flux.jl, MLJ.jl, ScikitLearn.jl
- **Visualization**: Plots.jl, Makie.jl, Gadfly.jl, VegaLite.jl
- **Differential Equations**: DifferentialEquations.jl
- **Optimization**: JuMP.jl, Optim.jl
- **Scientific Computing**: LinearAlgebra.jl, OrdinaryDiffEq.jl
- **Web**: HTTP.jl, Genie.jl, Mux.jl
- **Parallel Computing**: Distributed.jl, DistributedArrays.jl
- **Image Processing**: Images.jl, ImageFiltering.jl
- **Signal Processing**: DSP.jl, FFTW.jl
- **GPU Computing**: CUDA.jl, KernelAbstractions.jl
- **Testing**: Test.jl, SafeTestsets.jl
- **Documentation**: Documenter.jl
