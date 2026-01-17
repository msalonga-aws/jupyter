# Python 3.10 Kernel Setup for EMR Jupyter Notebooks

Automated script to install and configure a Python 3.10 kernel in Amazon EMR Jupyter notebook environments.

## Overview

This Jupyter notebook script automates the process of creating a Python 3.10 conda environment and registering it as a Jupyter kernel in EMR clusters. It handles the complexities of locating conda, creating isolated environments, and kernel registration.ddd

## What It Does

The script performs the following steps automatically:

1. **Locates Conda Installation** - Searches common EMR paths to find the conda executable
2. **Creates Conda Environment** - Sets up a new Python 3.10 environment in your home directory
3. **Installs Core Packages** - Adds essential data science libraries (pandas, numpy, matplotlib, scipy, jupyter)
4. **Registers Jupyter Kernel** - Makes the new Python 3.10 environment available as a kernel option
5. **Verifies Installation** - Confirms the kernel was registered successfully

## Installation

1. Open a Jupyter notebook in your EMR cluster
2. Create a new notebook with existing Python kernel
3. Copy and paste the entire script into a cell
4. Run the cell

## Usage

After running the setup script:

1. Click **Kernel** in the Jupyter menu
2. Select **Change kernel**
3. Choose **Python 3.10 (EMR)**
4. Your notebook will now use Python 3.10

If the kernel doesn't appear immediately, refresh the page or restart the Jupyter server.

## Environment Details

- **Environment Name**: `py310_kernel`
- **Environment Location**: `~/conda_envs/py310_kernel`
- **Kernel Name**: `py310`
- **Display Name**: Python 3.10 (EMR)

