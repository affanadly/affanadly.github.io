---
layout: post
title: Setting up Python and VS Code
date: 2024-03-31 12:00:00 +0800
tags: python vscode setup
categories: guide
---

This is how I setup my Python environment alongside Visual Studio Code (VS Code) on a fresh Windows/Linux installation.

## Python Installation

1. For Windows, download the latest Python installer from the [official website](https://www.python.org/downloads/windows). For Linux, Python is usually pre-installed, but if it isn't installed, you can install it using:

    ```bash
    sudo apt update
    sudo apt install python3 python3-pip
    ```

2. If in Linux, add the following to the `~/.bashrc` or `~/.profile` file:

    ```bash
    export PATH="$PATH:~/.local/bin"
    ```

3. Install the essential packages:

    ```bash
    pip install --default-timeout=100 matplotlib numpy pandas scipy sympy astropy tabulate uncertainties jupyter notebook ipympl ipykernel scikit-learn tqdm plotly
    pip install seaborn keras tensorflow cupy-cuda116 pysimplegui openpyxl # these are optional packages, install only if needed
    ```

## Visual Studio Code Installation

1. For Windows, download the latest VS Code installer from the [official website](https://code.visualstudio.com/download). For Linux, VS Code can be installed using the following commands:

    ```bash
    sudo apt-get install wget gpg
    wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
    sudo install -D -o root -g root -m 644 packages.microsoft.gpg /etc/apt/keyrings/packages.microsoft.gpg
    sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list'
    rm -f packages.microsoft.gpg
    
    sudo apt install apt-transport-https
    sudo apt update
    sudo apt install code
    ```
