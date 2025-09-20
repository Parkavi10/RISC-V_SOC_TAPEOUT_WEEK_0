# RISC-V Reference SoC Tapeout Program (VSD)

## 🛠️ Tool Installation Guide

All the instructions I followed for installing the required tools are provided below.(I have named my system Jey in Ubunutu-Virtual machine)

---

## **System Requirements**

- Minimum 6 GB RAM  
- At least 50 GB free HDD space  
- Ubuntu 20.04 or newer  
- 4 virtual CPU cores  

---
### **TOOL CHECK**

#### <ins>**Yosys**</ins>
```bash
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
$ git submodule update --init --recursive
$ make 
$ sudo make install
```


#### <ins>**Iverilog**</ins>
```bash
$ sudo apt-get update
$ sudo apt-get install iverilog
```


#### <ins>**gtkwave**</ins>
```bash
$ sudo apt-get update
$ sudo apt install gtkwave
```


