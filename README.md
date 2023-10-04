# Hugo Auto-Install Script for Linux

Note that this has currently only been tested on Amazon Linux 2023, but it should work on other flavors of linux too so long as they are using yum.

## Description

This repository contains a Bash script for automatically installing Hugo on Linux instances. The script is designed to be architecture-agnostic, supporting x86_64, aarch64, and 32-bit systems. It also allows for the installation of both the standard and extended editions of Hugo.

## Prerequisites

- Amazon Linux instance
- `sudo` privileges
- `wget` and `git` (these will be installed by the script if not already present)

## Usage

1. Clone this repository or download the script directly.
    ```bash
    git clone https://github.com/yourusername/hugo-auto-install.git
    ```
    or
    ```bash
    wget https://github.com/yourusername/hugo-auto-install/raw/main/hugo_install.sh
    ```

2. Make the script executable.
    ```bash
    chmod +x hugo_install.sh
    ```

3. Run the script.
    ```bash
    ./hugo_install.sh
    ```

## Configuration

The script uses two variables for configuration:

- `HUGO_VERSION`: The version of Hugo you want to install. Default is set to `0.119.0`.
- `HUGO_EDITION`: The edition of Hugo you want to install (`standard` or `extended`). Default is set to `extended`.

You can modify these variables directly in the script before running it.

## Contributing

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.
