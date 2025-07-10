# SSL Certificate Status Checker

A lightweight Python 3 tool that checks the SSL/TLS certificate details of any hostname and port.  
It displays expiration dates, issuer details, and days remaining — useful for system admins, DevOps, or anyone who needs to monitor certificates.

---

## ✅ Features

- Retrieves SSL certificate for any domain and port (default: 443)
- Displays:
  - Common Name (Issued To)
  - Issuer CN
  - Validity period (Not Before / Not After)
  - Days remaining until expiration
- Accepts single host via CLI or prompts interactively
- Supports custom ports (e.g., `example.com:8443`)
- Gracefully handles invalid input, DNS errors, and interruptions
- Cross-platform compatible (Windows, macOS, Linux)

---

## 🚀 Usage

### Run with a domain (one-time check)

```bash
python ssl_cert_status.py example.com
```

### Interactive mode (multiple lookups)

```bash
python ssl_cert_status.py
```

You’ll be prompted to enter hostnames (like `google.com` or `site.com:443`).  
To exit, type: `exit`, `quit`, or `q`.

---

## 📦 Requirements

- Python 3.6 or higher
- [`pyOpenSSL`](https://pypi.org/project/pyOpenSSL/)

Install via pip:

```bash
pip install pyOpenSSL
```

---

## 🔎 Sample Output

```
Enter server hostname or IP: google.com

SSL Certificate Information for google.com:443

  - Issued To:      *.google.com
  - Issuer:         GTS CA 1C3
  - Valid From:     2025-06-01 00:00:00+00:00
  - Valid Until:    2025-09-01 00:00:00+00:00
  - Days Remaining: 60 days
```

---

## 📁 File

- `ssl_cert_status.py` — Main script

---

## ⚖️ License

This project is licensed under the [MIT License](LICENSE)

---

## 🙋‍♂️ Author

Developed by [LuckyGitHub777](https://github.com/LuckyGitHub777)

Contributions, forks, and suggestions are welcome.
