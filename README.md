# 🔐 Data Governance & Privacy Protection in Python

This project showcases a complete data governance pipeline using Python — with a strong focus on **security, privacy, and validation**.  
It processes a dataset of passwords and applies several industry techniques including **anonymization**, **pseudonymization**, **encryption**, **role-based access control (RBAC)**, and even **classical cryptanalysis**.

---

## 🎯 Goals

- ✅ Data cleaning and validation using `pandera`
- 🔍 Sensitive data protection (GDPR/CCPA compliant)
- 🔐 Encryption using AES, Caesar cipher, and SHA-256
- 🧾 Logging access for HIPAA compliance
- ⚙️ Role-Based Access Control (RBAC)
- 🧠 Frequency analysis for Caesar cipher decryption

---

## 📦 Tools & Libraries

- **Pandas** - Data manipulation
- **Pandera** - Schema validation
- **PyCryptodome** - AES encryption
- **Hashlib** - SHA-256 hashing
- **Logging** - Secure access tracking
- **Matplotlib / Counter** - Frequency analysis
- **RBAC logic** - Role-based permissions

---

## 🔁 Workflow Summary

### 🧹 Step 1: Data Cleaning
- Fixing typos in `class_strength`
- Removing duplicate passwords
- Filtering out extreme values

### ✅ Step 2: Data Validation
Using `pandera` schema:
- Data types and allowed ranges
- Valid values for strength, length, entropy, etc.

### 🔐 Step 3: Security Measures
- **Anonymization**: SHA-256 hash of password
- **Pseudonymization**: Hashed identifiers (same as anonymization but with intended reversibility)
- **AES Encryption**: Encrypting password data using EAX mode
- **SHA-256 Hashing**: One-way secure hashing

### 🔏 Step 4: Access Logging & RBAC
- Log user actions with timestamps
- Implement access control for `admin` vs `user` roles

### 🔓 Step 5: Classical Encryption (Caesar)
- Encrypt passwords using Caesar Cipher
- Perform frequency analysis to reverse Caesar encryption
- Calculate similarity scores between original and decrypted texts

---

## 📈 Output Samples

| Password | Caesar Encrypted | Guessed Decryption | Similarity |
|----------|------------------|--------------------|------------|
| `abc123` | `def123`         | `abc123`           | 100%       |

---

## 🗂️ Project Structure

```
data-governance/
├── dataset.csv                    # Input dataset
├── main.py                        # Contains all logic (cleaning, security, RBAC)
├── access_log.txt                 # Access log file
├── README.md                      # This file
```

---

## 🧪 How to Run

1. ✅ Install required libraries:
```bash
pip install pandas pandera pycryptodome
```

2. ✅ Run the script in a Python IDE or Jupyter Notebook

3. ✅ Output will show:
   - Encrypted and anonymized values
   - Similarity between real and decrypted passwords
   - Access logs

---

## 🧑‍💻 Author

**Hossam Elsabbagh**  
📍 Zewail City of Science & Technology  
🎓 Computer Science & AI Student  

