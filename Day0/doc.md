
# VSD Hardware Design Program

## Tools Installation

#### <ins>All the instructions for installation of required tools can be found here:</ins>

### **System Requirements**
- 6 GB RAM  
- 50 GB HDD  
- Ubuntu 20.04 or higher (tested on Ubuntu 24.04 LTS)  
- 4 vCPU  

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
# Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. 
# Run the following command before running make:
$ git submodule update --init --recursive
$ make 
$ sudo make install
```

#### 📷 Image

<img width="862" height="592" alt="Image" src="https://github.com/user-attachments/assets/9f6d5606-0197-49d5-829f-c7e65a3867c7" />

---

#### <ins>**Iverilog**</ins>

```bash
$ sudo apt-get update
$ sudo apt-get install iverilog
```

#### 📷 Image

<img width="771" height="307" alt="Image" src="https://github.com/user-attachments/assets/6982aaf9-19be-4c9d-8eca-fed1f57591cd" />

---

#### <ins>**gtkwave**</ins>

```bash
$ sudo apt-get update
$ sudo apt install gtkwave
```

#### 📷 Image

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/8d0bd9f2-3fdc-497d-a8a0-d1c25b23c6e9" />

---

## Summary
- Installed **Yosys** for RTL synthesis  
- Installed **Icarus Verilog (iverilog)** for simulation  
- Installed **GTKWave** for waveform visualization  

This completes the basic toolchain setup for the VSD Hardware Design Program.

