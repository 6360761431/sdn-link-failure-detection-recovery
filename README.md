# SDN-Based Simulation of Link Failure Detection and Recovery Using Mininet

## Student Details
Name: Poojitha V  
SRN: PES2UG24AM113  

---

## Problem Statement
To simulate link failure detection and recovery in a network using Software Defined Networking (SDN) concepts in Mininet.

---

## Objective
- To design and implement a network topology using Mininet  
- To simulate link failure and recovery  
- To observe network behavior under failure conditions  
- To understand SDN concepts such as flow rules and controller-based decision making  

---

## Introduction to SDN
Software Defined Networking (SDN) is a networking paradigm that separates the control plane from the data plane. The control logic is centralized in a controller, which dynamically installs flow rules in network devices such as switches. This approach provides flexibility, programmability, and efficient network management.

---

## Topology Description
The network topology consists of:
- One switch (s1)  
- Three hosts (h1, h2, h3)  

Each host is connected to the switch, forming a simple star topology.

---

## Implementation

### Topology Creation
A custom topology is created using the Mininet Python API. The topology includes one switch and three hosts connected via links.

### Network Initialization
The Mininet network is started, and initial connectivity between all hosts is verified using:
pingall
This confirms that all hosts are reachable, with 0% packet loss.

### Link Failure Simulation
A link failure is simulated using the following command:

link s1 h1 down

This disconnects host h1 from the network. When connectivity is tested again, communication with h1 fails, resulting in packet loss.

### Link Recovery
The failed link is restored using:
link s1 h1 up

After restoration, connectivity is tested again, and all hosts successfully communicate with 0% packet loss.

## Observations
- Initial state: All hosts are reachable with no packet loss  
- During link failure: Communication with the disconnected host fails  
- After recovery: Network connectivity is restored successfully  

## Result
The network topology was successfully created using Mininet. Link failure was accurately simulated, resulting in communication loss. Upon restoring the link, full connectivity was re-established, demonstrating effective detection and recovery.

---

## Conclusion
This project demonstrates the detection and recovery of link failures in a network using Mininet. It also highlights fundamental SDN concepts such as packet handling, and controller-based decision making. The experiment shows how networks can dynamically adapt to topology changes.

---

## Screenshots
### Initial Connectivity
<img width="940" height="930" alt="image" src="https://github.com/user-attachments/assets/7fdd0194-dd3c-43d0-b67e-eebd2283a451"/>

### Ping Output
<img width="943" height="468" alt="image" src="https://github.com/user-attachments/assets/04f621ff-a0d5-4678-ba0e-34f7d73da584"/>

### Code
<img width="798" height="679" alt="image" src="https://github.com/user-attachments/assets/e1ed5d39-8daf-4897-91b8-9be00be5d3d9"/>

<img width="733" height="553" alt="image" src="https://github.com/user-attachments/assets/ec2d8067-2ad3-4c60-a96e-1be86808176d"/>

### cleanup
<img width="940" height="301" alt="image" src="https://github.com/user-attachments/assets/9cd09569-2d63-4394-9321-af89f075dc40"/>

### failure
<img width="940" height="395" alt="image" src="https://github.com/user-attachments/assets/bfb0bd8a-c1c7-47b0-b496-a332d84d9fd0"/>

### recovery
<img width="789" height="379" alt="image" src="https://github.com/user-attachments/assets/4b33efb2-b3a3-490f-9452-db2b4744113d"/>










