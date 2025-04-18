# Installing R Programming Language

This guide will walk you through the process of installing R and RStudio, the popular IDE for R development.

## System Requirements

- **Windows**: Windows 7 or later
- **macOS**: macOS 10.13 (High Sierra) or later
- **Linux**: Ubuntu 16.04 or later, Debian 9 or later, Red Hat/Fedora/CentOS 7 or later

## Installing R

### Windows

1. Go to the CRAN (Comprehensive R Archive Network) website: [https://cran.r-project.org/bin/windows/base/](https://cran.r-project.org/bin/windows/base/)
2. Click on the "Download R x.x.x for Windows" link (where x.x.x is the latest version)
3. Run the downloaded .exe file and follow the installation instructions

### macOS

1. Go to the CRAN website: [https://cran.r-project.org/bin/macosx/](https://cran.r-project.org/bin/macosx/)
2. Download the latest R package (.pkg file)
3. Open the downloaded file and follow the installation instructions

### Linux (Ubuntu/Debian)

```bash
# Add the CRAN repository
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9
sudo add-apt-repository 'deb https://cloud.r-project.org/bin/linux/ubuntu focal-cran40/'

# Update packages and install R
sudo apt update
sudo apt install r-base r-base-dev
```

### Linux (Fedora/CentOS/RHEL)

```bash
# For Fedora
sudo dnf install R

# For CentOS/RHEL
sudo yum install epel-release
sudo yum install R
```

## Installing RStudio (Recommended IDE)

RStudio is the most popular IDE for R development and provides a user-friendly interface with many helpful features.

1. Go to the RStudio download page: [https://www.rstudio.com/products/rstudio/download/#download](https://www.rstudio.com/products/rstudio/download/#download)
2. Select the appropriate installer for your operating system
3. Run the installer and follow the installation instructions

## Verifying Installation

### Command Line

Open a terminal or command prompt and run:

```bash
R --version
```

You should see the installed R version information.

### Running R

- **Windows**: Open RStudio from the Start menu or run R from the command prompt
- **macOS**: Open RStudio from Applications or run R from Terminal
- **Linux**: Open RStudio from your applications menu or run R from the terminal

## Installing Essential Packages

Once R is installed, you can install some essential packages using the R console:

```r
# Install the tidyverse collection of packages (ggplot2, dplyr, tidyr, etc.)
install.packages("tidyverse")

# Install RMarkdown for report generation
install.packages("rmarkdown")

# Install Shiny for interactive web applications
install.packages("shiny")
```

## Troubleshooting

- **Package installation errors**: Make sure you have the required system dependencies. On Linux, you may need to install additional development libraries.
- **Permission issues**: On Linux and macOS, you might need to use `sudo` for system-wide installations.
- **RStudio doesn't detect R**: Make sure R was installed before RStudio.
