
# 🔐 Password Cracking with John the Ripper – W3-PM1

## 📌 Project Overview

As part of **Week 3 (W3-PM1)** of the **Networkwalks Cybersecurity & Ethical Hacking Internship**, I performed a practical exercise on password recovery of a password-protected PDF using **John the Ripper** and **Johnny GUI**.

The main objective was to understand PDF hash extraction, password cracking, and verification of the recovered password.

> ⚠️ This activity was performed in an authorized cybersecurity training environment.

---

## 🎯 Objectives

- Extract the password hash from a protected PDF.
- Understand the role of `pdf2john`.
- Import the extracted hash into Johnny.
- Perform password recovery using John the Ripper.
- Verify the recovered password.
- Unlock the PDF and capture the challenge flag.

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **pdf2john / Online HashCrack** | Extract PDF password hash |
| **John the Ripper** | Password recovery |
| **Johnny GUI** | Graphical frontend for John the Ripper |
| **PDF Reader / Microsoft Edge** | Password verification |

---

## 🔬 Practical Methodology

### 🔹 1. Target Identification

The target used during the practical was:

```text
My Locked PDF1.pdf
```

The PDF was password protected and required a password to access its contents.

---

### 🔹 2. PDF Hash Extraction

The protected PDF was processed using a `pdf2john` extraction utility.

The extracted hash started with:

```text
$pdf$4*4*128*...
```

The extracted hash was saved locally as:

```text
hash1.txt
```

**Flow:**

```text
Protected PDF → pdf2john → PDF Hash → hash1.txt
```

---

### 🔹 3. Hash Import into Johnny

The extracted `hash1.txt` file was imported into **Johnny**.

The target was recognized as a PDF hash:

```text
Format: PDF
```

The password recovery process was then started.

---

### 🔹 4. Password Recovery

John the Ripper successfully recovered the password:

```text
good-luck
```

Cracking status:

```text
100% cracked
```

---

### 🔹 5. Password Verification

The recovered password was entered into the protected PDF:

```text
good-luck
```

The PDF successfully opened, confirming that the recovered password was correct.

---

### 🔹 6. Flag Capture

After unlocking the PDF, the following challenge flag was obtained:

```text
nw{cybersecurity_flag_captured_2608}
```

---

## 📊 Results

| Activity | Result |
|---|---|
| PDF Hash Extraction | ✅ Successful |
| Hash Import | ✅ Successful |
| Password Recovery | ✅ Successful |
| Recovered Password | `good-luck` |
| PDF Unlock | ✅ Successful |
| Flag Capture | ✅ Successful |

---

## 🧠 Key Concepts Learned

- PDF password protection
- PDF hash extraction using `pdf2john`
- John the Ripper
- Johnny GUI
- Password recovery techniques
- Weak password security
- Basic encryption and hashing concepts

---

## 🛡️ Security Recommendations

- Use long and unique passwords for sensitive documents.
- Avoid common words and predictable phrases.
- Do not reuse passwords across multiple systems or documents.
- Use modern encryption mechanisms where available.
- Restrict access to sensitive documents.

---

## 📸 Evidence

### 1. PDF Hash Extraction

![PDF Hash Extraction](screenshots/01-pdf-hash-extraction.png)

### 2. Hash Imported into Johnny

![Johnny Hash Import](screenshots/02-johnny-hash-import.png)

### 3. Password Successfully Cracked

![Password Cracked](screenshots/03-password-cracked.png)

### 4. Password Verification

![Password Verification](screenshots/04-password-verification.png)

### 5. Challenge Flag Captured

![Flag Captured](screenshots/05-flag-captured.png)

---

## 👨‍💻 Internship Details

**Author:** Gopal Mahajan  
**Program:** Networkwalks Cybersecurity & Ethical Hacking Internship  
**Batch:** B083-Networkwalks  
**Week:** 3  
**Module:** W3-PM1  
**Project:** Password Cracking with John the Ripper

---

## ⚠️ Ethical Disclaimer

This practical was performed only in an authorized cybersecurity training environment. Password-cracking techniques should only be used against files or systems that you own or have explicit permission to test.

### ✅ Status

**Successfully Completed**
