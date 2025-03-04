# SHA-1 Password Cracker

## 📌 Overview

This project is a **SHA-1 password cracker** that attempts to retrieve the original plaintext password from a given SHA-1 hash. It works by comparing the hash against a precomputed list of common passwords. The program also supports **salting** to check for passwords that have been hashed with known salts.

---

## 🔥 Features

- **Cracks SHA-1 hashed passwords** by comparing against a wordlist.
- **Supports salting** (optional) to check for hashes that include known salts.
- **Uses a dictionary attack** method with a large password list (`10-million-password-list-top-10000.txt`).
- **Fast and efficient**—performs hashing and comparison in an optimized way.

---

## 🛠️ Requirements

Ensure you have **Python 3.x** installed on your system.  
You can check your Python version with:

```sh
python --version
```

### **Python Libraries Used**
- `hashlib` (Built-in)

No external dependencies are required.

---

## 🚀 Installation & Setup

1. **Clone the Repository** (or download the script):
   ```sh
   git clone https://github.com/kinza099/SHA-1-Password-Cracker-using-Python.git
   cd SHA-1-Password-Cracker-using-Python
   ```

2. **Prepare the Required Files**:
   - `10-million-password-list-top-10000.txt`: A wordlist of common passwords.
   - `known-salts.txt`: A file containing common salts (optional for salted hashes).

---

## 🎯 Usage

Run the program with a SHA-1 hash to check if it exists in the dictionary.

### **Basic Usage (Without Salting)**
```sh
python sha1_cracker.py
```
Enter the **SHA-1 hash** when prompted, and the program will attempt to find the matching password.

### **Example**
```python
print(crack_sha1_hash("b1b3773a05c0ed0176787a4f1574ff0075f7521e"))
```
**Output:**
```
hello
```

---

## 🔑 Using Salts

To check for **salted** passwords, modify the script to use salts.

Example:
```python
crack_sha1_hash("some_sha1_hash", use_salts=True)
```
This will check both **prepended** and **appended** salts.

---

## 🗂 File Structure

```
sha1-password-cracker/
│── ShA1_pass_cracker.py   # Main Python script
│── 10-million-password-list-top-10000.txt # Wordlist of common passwords
│── known-salts.txt        # List of salts (optional)
│── README.md              # Documentation
```

---

## 🛡️ Disclaimer

This tool is intended for **educational and ethical** purposes only.  
Do **not** use it for illegal activities. The author is **not responsible** for any misuse.

---

## 👨‍💻 Author

- **Kinza Bughio**  
- GitHub: [kinza099](https://github.com/kinza099)
- LinkedIn: [LinkedIn](www.linkedin.com/in/kinza-bughio-782777279)

---

## 📝 License

This project is licensed under the **MIT License**. Feel free to modify and distribute it. 🎯


