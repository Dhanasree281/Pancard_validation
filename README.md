# 🧹 PAN Data Cleaning & Validation with Python  

This project focuses on **cleaning, validating, and handling Permanent Account Number (PAN)** data using Python.  
It is designed as a **real-world style data cleaning project** to strengthen skills in Python, regular expressions, and data preprocessing.  

---

## 📌 Features  
- ✅ Clean messy PAN number data  
- ✅ Validate PAN numbers using **Regex**  
- ✅ Handle **missing or invalid** PAN values  
- ✅ Write **reusable validation functions**  
- ✅ Ready-to-use for integration with real-world datasets  

---

## 🧾 PAN Number Format (India)  
- A valid PAN number is a **10-character alphanumeric string**:  
  - First 5 characters → **Uppercase letters (A–Z)**  
  - Next 4 characters → **Digits (0–9)**  
  - Last character → **Uppercase letter (A–Z)**  
- Example: `ABCDE1234F`  

Regex pattern used in this project:  

```python
^[A-Z]{5}[0-9]{4}[A-Z]{1}$
📦 PAN-Data-Cleaning
 ┣ 📜 pan_cleaning.py     # Main Python script
 ┣ 📜 requirements.txt    # Required dependencies
 ┣ 📜 sample_data.csv     # Example dataset
 ┗ 📜 README.md           # Project documentation

from pan_cleaning import validate_pan

print(validate_pan("ABCDE1234F"))  # ✅ Valid
print(validate_pan("abc123"))      # ❌ Invalid


