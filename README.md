# xIPL, Cross-platform (x) Installer, Patcher, and Launcher (IPL)

The **xIPL** is a fancy **bash** script designed to automate the **I**nstallation, **P**atching, and **L**aunching of Ultima Online. Targeted at the shard Shadow Age: REBORN, this software aims to be compatible with Linux, BSD, and MacOS (Intel-base Processors) along with MacOS (M1/M2 Processors).

## Features
- Cross-platform, tested in Linux (Intel 64-bit) and MacOS (ARM M2)
- xIPL auto-updates itself.
- Auto-configures settings.
- Installs / Patches client
- Launches client

## TODO
- Optimize WINETRICKS package checking or...
- **-skip** command for Winetricks.
- Preserve backup of macro profiles.
- Persistent settings between patches: ClassicUO/settings.json

### Requirements

- **Perl** - This is used to replace text in some of the registry files for Wine since **sed**'s behaviour is platform dependent.
- **Git** - Used to download and update additional dependencies.
- **Python** - Minimum of Python 3 version __**3.9.1**__
- **Brew** - (MacOS) Used for the installation of WINE and WINETRICKS.
- **curl** or **wget** - Used for auto-updating the xIPL.
- **Wine** - Run the ClassicUO client. Downloaded automatically for MacOS, package provided by [Gcenx/homebrew-wine](https://github.com/Gcenx/homebrew-wine)
- **Winetricks** - Download and install additional required packages for Wine. Downloaded automatically for MacOS, package provided by [Gcenx/homebrew-wine](https://github.com/Gcenx/homebrew-wine)

### Dependencies

- **uopatcher** - Downloaded automatically and used for **patching** of the client, provided by [Ohkthx/uopatcher](https://github.com/ohkthx/uopatcher).

### Installation

It is ideal to store the installation script in its own directory, below provides commands to create that directory in the terminal and switch to it. The method to downloading the client is up to you. You can use **curl**, **wget**, or just copy the raw file from the browser. **curl** and **wget** commands are provided below.

```bash
# Create a directory and enter it for the installation.
mkdir xIPL
cd xIPL

# Obtaining the xIPL with CURL
curl -O https://raw.githubusercontent.com/Ohkthx/xIPL/main/xIPL

# Obtaining the xIPL with WGET
wget https://raw.githubusercontent.com/Ohkthx/xIPL/main/xIPL

```

### Running

To start the **xIPL**, you just need to type the following. In additional to normal execution, provided are **OPTIONAL** steps to make the script executable and started with using `./xIPL`
```bash
# Start with bash.
bash xIPL

# OPTIONAL: Make it executable and be able to run with ./xIPL
chmod +x xIPL
./xIPL
```
