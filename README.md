# 🚚 Automated Warehouse using PLC (CPU 313C-2 DP) and Factory I/O 🏭

## 📖 Project Overview
This project demonstrates the automation of a **warehouse system** using a **Siemens S7-300 PLC (CPU 313C-2 DP)** and **Factory I/O** for simulation. The system automates the storage, retrieval, and handling of items in a warehouse by controlling conveyors, sensors, and actuators. The project supports both **Auto** and **Manual** modes.


## 🖥 Hardware Used

- **PLC**: Siemens S7-300 CPU 313C-2 DP
- **Software**: TIA Portal (Step 7)
- **Factory I/O**: Simulation platform for real-time monitoring and control

## ⚙️ System Operation Logic

The warehouse system operates based on the following sequence:

| Condition               | Action                             |
|-------------------------|------------------------------------|
| Item detected at entry  | ✅ Open conveyor to move item      |
| Item reaches storage position | ✅ Close conveyor (store item) |
| Stop button pressed      | ❌ All outputs OFF (safe state)    |
| Manual mode              | Operator can control conveyors and storage from Factory I/O |
| Auto Mode                | Automatic item handling based on sensor inputs |

## 🔧 Features

- **Automatic item movement**: The system automatically moves items from the entry point to storage locations.
- **Manual override**: The operator can manually control conveyors and devices via Factory I/O.
- **Start / Stop pushbuttons**: Allows for manual operation and emergency stop functionality.
- **Simulation support**: The system is fully simulated using Factory I/O, where the PLC interacts with the virtual environment.

## 🛠 PLC Design

The PLC program is created using **TIA Portal** and includes:

- **Ladder Logic (LAD)** for control of item movement and system functionality.
- Control for conveyors, sensors, and actuators in the warehouse.

## 🏗 Factory I/O Design

In **Factory I/O**, the system consists of:

- **Conveyors**: Move items between different locations within the warehouse.
- **Storage units**: Represent areas where items are stored after being moved.
- **Sensors**: Detect the position of items on conveyors and trigger PLC actions.
- **Actuators**: Controlled by the PLC to operate conveyors and other devices based on sensor inputs.

### 🖥 Factory I/O Screens

1. **System Overview**: Displays a graphical representation of the warehouse, with live status for each conveyor and storage unit.
2. **Control Panel**: Allows for manual control of conveyors and storage units.


## 📂 Project Files

- **PLC Program**: Written in LAD using TIA Portal.
- **Factory I/O Scene File**: Includes warehouse layout and components simulated in Factory I/O.

## 🚀 How to Run

Clone the repository:
 
     git clone https://github.com/yourusername/Automated-Warehouse-Using-PLC.git
     cd Automated-Warehouse-Using-PLC

## 📷 Project Architecture
![Automated WareHouse](https://github.com/nrasel/Automated-WireHouse-Using-PLC-and-Factory-IO/blob/47da809f59122e3a4172d0c54128a32166964209/FlowChart%20of%20this%20Project.PNG)







