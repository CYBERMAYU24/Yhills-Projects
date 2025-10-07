
# 🕵️‍♂️ Packet Sniffer and Analysis Tool

A Python-based **Network Packet Sniffer and Analyzer** built using **Scapy** and **Tkinter**.  
This tool captures, inspects, and analyzes live network packets in real time.  
It highlights suspicious activity, supports custom filters, and generates detailed reports.

---

## 📖 Features

### 🧩 Packet Capture
- Captures live packets using **Scapy**.
- Displays key details — Source, Destination, Protocol, Length, and Info.

### 🔍 Filtering
- Apply custom filters (e.g., `tcp`, `udp`, `icmp`, or any keyword).

### 🧠 Packet Analysis
Automatically analyzes each packet for:
- Known **malicious IP addresses**.  
- **High traffic rate** from the same source.  
- **Oversized packets** (possible flooding or data exfiltration).

Suspicious packets are highlighted in **red** with alert messages.

### 🪟 GUI Interface
- Built using **Tkinter** for easy visualization.  
- Packet list view with color-coded rows.  
- Packet **Details** (header info) and **Hex View** for deep inspection.

### 🧾 Report Generation
- Generates a detailed `.txt` report containing:
  - Total packets captured  
  - Unique sources  
  - List of suspicious packets  
- Example:  
```

---

## ⚙️ Requirements

| Requirement | Description |
|--------------|-------------|
| **Python** | 3.8 or higher |
| **Libraries** | `scapy`, `tkinter`, `threading`, `queue` |
| **Platform** | Works on Windows and Linux (Kali recommended) |

Install Scapy if not already installed:
```bash
pip install scapy
````

---

## 🚀 How to Run

1. Clone or download the project:

   ```bash
   git clone https://github.com/yourusername/packet-sniffer-tool.git
   cd packet-sniffer-tool
   ```
2. Download the zip file here and make sure you have all the requirements satisfied =
   https://github.com/CYBERMAYU24/Yhills-Projects/releases/tag/v1 

3. Run the script:

   ```bash
   python packet_sniffer.py
   ```

4. Select the desired **network interface** from the dropdown.

5. Click **Start** to begin capturing packets.

6. Apply filters or click **Generate Report** after analysis.

---

## 🧰 Project Structure

```
packet-sniffer-tool/
│
├── packet_sniffer.py       # Main GUI and core logic
├── README.md               # Documentation
├── captured/               # (Optional) Folder for saved .pcap files
└── reports/                # (Optional) Folder for generated reports
```

---

## 📊 Analysis Logic

| Check Type           | Description                   | Example Alert           |
| -------------------- | ----------------------------- | ----------------------- |
| **Malicious IP**     | Matches against known bad IPs | `Malicious IP detected` |
| **High Traffic**     | Same source sends >50 packets | `High traffic rate`     |
| **Oversized Packet** | Size > 1500 bytes             | `Oversized packet`      |

---

## 📸 Preview 

<img width="1920" height="936" alt="Screenshot_2025-10-07_05_40_33" src="https://github.com/user-attachments/assets/a4f7aada-78ce-4fbf-8825-421ff6cf40a9" />



## 🏁 Conclusion

This tool demonstrates how **Python**, **Scapy**, and **Tkinter** can be used together to create a functional and interactive **network security analysis tool**.
It serves as a beginner-friendly introduction to **packet analysis** and **network monitoring** concepts.

---

## 👨‍💻 Author

**Mayur Gajbhiye**
*Developed as part of a cybersecurity internship project.*
📅 *October 2025*

```
