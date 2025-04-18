# Yorick Installation Guide

## Required Software

- **Yorick**: Interpreted programming language for scientific computing
- **C Compiler**: GCC or Clang for building Yorick from source
- **Make**: Build automation tool
- **X11 Development Libraries**: For graphical output
- **Emacs**: With yorick-mode (optional)
- **VS Code**: With custom configuration for Yorick (optional)
- **GFortran**: For certain numerical packages (optional)

## File Extensions

- `.i` - Yorick source files
- `.i0` - Yorick autoload function definition files
- `.i1` - Yorick binary data files
- `.info` - Yorick package information files
- `.eps` - PostScript graphics output
- `.ps` - PostScript graphics output
- `.cgm` - Computer Graphics Metafile output
- `.so`, `.dll` - Dynamically loaded plugin files
- `.c`, `.h` - C source files for compiled plugins
- `.f`, `.f90` - Fortran source files for compiled plugins
- `.o` - Compiled object files
- `Makefile` - Build configuration

## Package Management

```bash
# Yorick doesn't have a standard package manager
# Packages are typically installed manually

# Clone a package repository
git clone https://github.com/username/yorick-package.git

# Build and install a package
cd yorick-package
make
make install

# Install a package to user directory
make install DEST_Y=~/yorick

# Create a symbolic link in Yorick package directory
ln -s ~/path/to/yorick-package /usr/local/lib/yorick/packages/packagename

# Check for installed packages in Yorick
yorick -batch -i "help, plug_dir"
```

## Running Yorick Programs

```bash
# Start Yorick interpreter
yorick

# Run a Yorick script
yorick -i script.i

# Run in batch mode (no interactive prompt)
yorick -batch -i script.i

# Run with custom include path
yorick -i script.i -I /path/to/include

# Pass arguments to script
yorick -i script.i arg1 arg2

# Execute a Yorick expression
yorick -batch -i 'print, "Hello, World!"'

# Create a custom executable
cd ~/yorick-package
make yor-custom

# Run the custom executable
./yor-custom

# Generate documentation
yorick -batch -i "help, fullhelp"
```

## Common Libraries

- **Matrix Operations**: Built-in array and matrix functions
- **File I/O**: Binary and text file operations
- **Graphics**: 2D plotting and visualization
- **FFT**: Fast Fourier Transform
- **HDF5**: HDF5 file format support
- **NetCDF**: NetCDF file format support
- **FITS**: FITS astronomy file format
- **SPy**: Signal processing
- **MPI**: Message Passing Interface for parallel computing
- **YETI**: Extended matrix operations
- **YOSSI**: Yorick OpenScientific Software Interface
- **YURL**: URL and network support
- **YGSL**: GNU Scientific Library interface
- **YIMUTIL**: Image utilities
- **YORICK-Z**: Compression support
- **YORICK-OPTIMPACK**: Optimization package
