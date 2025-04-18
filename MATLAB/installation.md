# MATLAB Installation Guide

## Required Software

- **MATLAB**: The commercial MATLAB environment from MathWorks
- **GNU Octave**: Free open-source alternative to MATLAB
- **Toolboxes**: Optional MATLAB toolboxes for specific domains
- **MATLAB Runtime**: For deploying standalone applications
- **MATLAB Engine for Python**: For integrating with Python

## File Extensions

- `.m` - MATLAB/Octave code files
- `.mat` - MATLAB data files
- `.fig` - MATLAB figure files
- `.p` - Obfuscated MATLAB files
- `.mlx` - MATLAB Live Scripts
- `.slx` - Simulink model files
- `.mdl` - Legacy Simulink model files
- `.mex*` - MATLAB executable files (platform-specific extensions)
- `.mlapp` - MATLAB app files
- `.mlappinstall` - MATLAB app installation files
- `.mlpkginstall` - MATLAB package installation files

## Package Management

```bash
# MATLAB Add-On Explorer (GUI)
# In MATLAB, navigate to Home > Add-Ons > Get Add-Ons

# MATLAB command-line package management
# Install an add-on from file
matlab.addons.install('addon.mlpkginstall')

# Uninstall an add-on
matlab.addons.uninstall('PackageName')

# List installed add-ons
matlab.addons.installedAddons()

# For Octave:
# Install a package
pkg install -forge package_name

# Load a package
pkg load package_name

# Update all packages
pkg update
```

## Running MATLAB Programs

```bash
# Start MATLAB GUI
matlab

# Start MATLAB in command-line mode
matlab -nodesktop

# Run a specific script
matlab -r "run('script.m'); exit"

# Run with arguments
matlab -r "arg1='value1'; arg2='value2'; run('script.m'); exit"

# Run with no splash screen and no Java VM
matlab -nosplash -nojvm -r "run('script.m'); exit"

# For Octave:
# Start Octave GUI
octave --gui

# Run an Octave script
octave script.m

# Run Octave non-interactively
octave --no-gui --eval "source('script.m')"
```

## Common Libraries/Toolboxes

- **Signal Processing Toolbox**: Digital and analog signal processing
- **Image Processing Toolbox**: Image analysis and algorithm development
- **Statistics and Machine Learning Toolbox**: Data analysis and modeling
- **Optimization Toolbox**: Solving optimization problems
- **Control System Toolbox**: Analyze and design control systems
- **Deep Learning Toolbox**: Create and train neural networks
- **Financial Toolbox**: Financial modeling and analysis
- **Parallel Computing Toolbox**: Parallel processing and GPU computing
- **Simulink**: Model and simulate dynamic systems
- **Communications Toolbox**: Design communications systems
- **Robotics System Toolbox**: Design and test robot algorithms
