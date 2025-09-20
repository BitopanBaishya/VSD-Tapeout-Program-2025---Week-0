# Week 0: Environment Setup & Installation of Tools.
 
The focus of this week is on **installing and verifying the required tools** in a Linux environment.

---

## 📑 Objectives
- Install the following tools:
    * Oracle VirtualBox (for running Linux)
    * Yosys
    * Iverilog
    * GTKWave
- Verify successful installation and environment setup.
- Document the process with clear steps, logs, and screenshots.

---

## 🛠️ Installation Steps
<details>
  <summary>Oracle VirtualBox</summary>
 
We need to install the Oracle VirtualBox for running the Linux environment in Windows or MAC OS.

🔗 [Download VirtualBox from here.](https://www.virtualbox.org/wiki/Downloads)

We also need to download the Ubuntu ISO file for installation in Oracle VirtualBox.

🔗 [Download Ubuntu from here.](https://ubuntu.com/download/desktop)

  Then setup the following system in VirtualBox:
  - Ubuntu 20.04+
  - 6GB RAM, 50 GB HDD
  - 4vCPU
</details>

<details>
 <summary>Yosys</summary>
 Run the following commands in the terminal:
 
 ```
sudo apt-get update 
git clone https://github.com/YosysHQ/yosys.git 
cd yosys 
sudo apt install make (If make is not installed please install it)  
sudo apt-get install build-essential clang bison flex libreadline-dev gawk tcl-dev libffi-dev git graphviz xdot pkg-config python3 libboost-system-dev libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc 
make  
sudo make install
 ```
 To verify successful installation, run:

```
yosys --version
```
</details>

<details>
 <summary>Iverilog</summary>
 Run the following commands in the terminal:
 
 ```
sudo apt-get update 
sudo apt-get install iverilog 
 ```
 To verify successful installation, run:

```
iverilog -v
```
</details>

<details>
 <summary>GTKWave</summary>
 Run the following commands in the terminal:
 
 ```
sudo apt-get update 
sudo apt install gtkwave 
 ```
 To verify successful installation, run:

```
gtkwave -v
```
</details>
