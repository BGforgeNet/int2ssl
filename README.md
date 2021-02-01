# int2ssl
[![windows](https://github.com/BGforgeNet/int2ssl/workflows/msbuild/badge.svg)](https://github.com/BGforgeNet/int2ssl/actions?query=workflow%3AMSBuild)
[![linux](https://github.com/BGforgeNet/int2ssl/workflows/cmake/badge.svg)](https://github.com/BGforgeNet/int2ssl/actions?query=workflow%3ACMake)
[![Discord](https://img.shields.io/discord/401990446747877376.svg)](https://discord.gg/jxs6WRq)

Script decompiler for Fallout 1/2.

- Originally implemented by **Anchorite** (2005-2009).
- Rewritten for multiple platform support by [*alexeevdv*](https://github.com/alexeevdv) (2015).
- Expanded for full [*sfall*](https://github.com/phobos2077/sfall) support by [*Nirran*](https://github.com/nirran), [*phobos2077*](https://github.com/nirran), [*Mr.Stalin*](https://github.com/FakelsHub) (2014-2020).

- [Installation](#installation)
  - [Windows](#windows)
  - [Ubuntu](#ubuntu)
  - [Other Linux](#other-linux)
  - [Building from source](#bilding-from-source)
- [Usage](#usage)
- [Changelog](CHANGELOG.md)


## Installation

### Windows

Download `int2ssl.exe` from the [latest release](https://github.com/BGforgeNet/int2ssl/releases/latest) page.

### Ubuntu

```bash
sudo add-apt-repository ppa:bgforge.net/ppa
sudo apt install int2ssl
```

### Other Linux
Download `int2ssl` binary from the [latest release](https://github.com/BGforgeNet/int2ssl/releases/latest) page.

### Building from source

Dependencies: Cmake (>=2.8).

```bash
mkdir build && cd build && cmake .. && make
```

## Usage

```
Usage: ./int2ssl [options] [-s value] file.int [file.ssl]
Example: ./int2ssl -d-1-a-b-e-s3 random.int

Options
  -d: dump file
  -1: input file is Fallout 1 script
  -a: ignore wrong number of arguments
  -b: insert omitted arguments backward
  -s: use Space instead of tab to indent
  -e: stop decompiling on error
  --: end of options
```
