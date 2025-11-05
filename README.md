# WiFi Performance Lab

This project analyzes **Wi-Fi and Ethernet network performance** using **iperf3** and **Wireshark**, comparing real and theoretical **goodput** across different setups.  
It was developed as part of the **Wireless Security** course at **Politecnico di Torino**, taught by *Prof. Marco Mellia*.

---

## 🧠 Overview
The lab evaluates **TCP and UDP throughput** under six scenarios:
1. WiFi ↔ WiFi (TCP)
2. WiFi ↔ WiFi (UDP)
3. WiFi ↔ Ethernet (TCP)
4. WiFi ↔ Ethernet (UDP)
5. Ethernet ↔ Ethernet (TCP)
6. Ethernet ↔ Ethernet (UDP)

A **Python automation script** executes multiple `iperf3` sessions and computes statistical performance metrics (mean, min/max, standard deviation).

---

## ⚙️ Tools & Setup
- **OS:** Kali Linux (Debian-based)
- **Tools:** iperf3, Wireshark  
- **Hardware:**  
  - Access Point: Technicolor DGA4331TIM  
  - Client: ASUS TUF Dash F15 (Wi-Fi 6)  
  - Server: MSI Pulse GL66 (Wi-Fi 6 / Ethernet)  
  - Cable: Cat 5e UTP (1 Gbps)

---

## 📈 Key Findings
- Wi-Fi performance is limited by **half-duplex** and **interference**.  
- Ethernet achieves results close to the theoretical 1 Gbps limit.  
- Hybrid WiFi–Ethernet connections reduce wireless bottlenecks.  
- Environmental factors (e.g., metallic barriers) significantly impact throughput.

---

## 📂 Repository Structure
```plaintext
wifi-performance-lab/
│
├── wifi_performance.py   # Python automation script (iperf3 tests)
├── report.pdf            # Full lab report
└── README.md             # Project overview
