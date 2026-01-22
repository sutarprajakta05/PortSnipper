# 🔍 PortSnipper

PortSnipper is a simple Python-based TCP port scanner that scans a target host for open ports.  
It is designed for **learning, basic reconnaissance, and security testing** purposes.

> ⚠️ Use only on systems you own or have permission to scan.

---

## 🚀 Features

- Scan TCP ports **1–5000**
- Fast and lightweight
- Written in **Python 3**
- Clean output with scan timing
- Handles common errors (Ctrl+C, DNS issues, connection errors)

---

## 🛠️ Requirements

- Linux (Kali, Ubuntu, etc.)
- Python **3.x**

Check Python version:
```bash
python3 --version
```
📦 Installation

Clone the repository:
```bash
git clone https://github.com/sutarprajakta05/PortSnipper.git
cd PortSnipper
```
▶️ Usage

Run the scanner:
```bash
python3 PortSnipper.py
```
Enter the target host when prompted:
```bash
Enter a remote host to scan: testphp.vulnweb.com
```
📌 Example Output
```
___________________________________________________________
Please wait, scanning remote host 44.228.249.3
____________________________________________________________
Port 80:      Open
Port 443:     Open
Scanning Completed in:  0:00:08.342190
```
⚙️ How It Works

- Resolves hostname to IP using socket.gethostbyname()
- Iterates through ports 1–5000
- Uses TCP connect scan (socket.connect_ex)
- Records total scan time using datetime

🧠 Limitations

- Single-threaded (slower than tools like Nmap)
- TCP connect scan only
- No service/version detection

📌 Future Improvements

- Multithreading for faster scans
- Custom port range support
- Service detection
- Output to file
- Banner grabbing

⚠️ Disclaimer

- This tool is intended for educational purposes only.
- The author is not responsible for misuse or illegal activities.

👤 Author

Prajakta Sutar
- GitHub: https://github.com/sutarprajakta05
