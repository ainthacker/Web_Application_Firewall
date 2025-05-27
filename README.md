# 🚀 Web Application Firewall (WAF)

A lightweight and robust Web Application Firewall (WAF) designed to protect your web applications from common attacks. Developed from scratch in just 24 hours during a Hackathon event.

![image](https://github.com/user-attachments/assets/9d186bf7-d811-4732-a8d6-c9e87719824c)



---

## 🛡️ Features
- SQL Injection detection and prevention
- XSS (Cross-Site Scripting) attack detection
- Simple DoS protection (request rate limiting)
- Attack logging in a local database
- User authentication and session management
- Clean and modern user interface

---

## ⚙️ Installation

1. **Create a Python Virtual Environment**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```
2. **Install Required Packages**
    ```bash
    pip install -r requirements.txt
    ```
3. **Start the Server**
    ```bash
    python Server.py
    ```
    The server will run by default at [http://localhost:5000](http://localhost:5000)

---

## 🗄️ Database
- Database: `waf.db` (SQLite)
- To view attack logs:
    ```bash
    sqlite3 waf.db
    SELECT * FROM attacks;
    ```

---

## 📁 Project Structure
```
├── Server.py           # Main server and application logic
├── AttackTest.py       # Attack detection and logging
├── SQLi.py             # SQL Injection detection
├── XSS.py              # XSS detection
├── DOS.py              # DoS protection
├── requirements.txt    # Python dependencies
├── Templates/          # HTML templates
└── README.md           # Project documentation
```

---



## 📬 Contribution & Contact
Contributions and feedback are welcome! Please open an issue or submit a pull request if you have suggestions or improvements.
