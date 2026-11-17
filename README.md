# NETWORKWALKS-FeliciaObinnaAmadi-B084-WK3-PM1-PM2-PASSWORD-CRACKING
# Password Cracking & Hash Recovery Lab

## 📌 Project Overview
This repository documents hands-on lab exercises focused on password recovery, hash extraction, and dictionary-based cracking techniques. The project demonstrates how security professionals evaluate password strength and test document encryption robustness using **John the Ripper (JTR)**, **Johnny GUI**, and custom browser-based utility tools[span_14](start_span)[span_14](end_span)[span_15](start_span)[span_15](end_span).

---

## 🛠️ Tools & Technologies Used
* **John the Ripper (JTR) / Johnny:** Industry-standard password security auditing and recovery tool (CLI & GUI implementation on Windows)[span_16](start_span)[span_16](end_span)[span_17](start_span)[span_17](end_span).
* **Networkwalks Hash Calculator & Password Cracker:** Browser-based utilities for parsing encrypted PDF files and running wordlist dictionary checks[span_18](start_span)[span_18](end_span)[span_19](start_span)[span_19](end_span).
* **Environment:** Windows host environment utilizing local binary execution (`john.exe`) and text-based hash management (`hash1.txt`)[span_20](start_span)[span_20](end_span)[span_21](start_span)[span_21](end_span).

---

## ⚙️ Methodology & Step-by-Chief Implementation

### Module 1: CLI & GUI Cracking with John the Ripper
1. **Binary Setup:** Downloaded and configured John the Ripper Jumbo binaries (`john.exe`) alongside the Johnny GUI interface[span_22](start_span)[span_22](end_span)[span_23](start_span)[span_23](end_span).
2. **Hash Extraction:** Extracted the secure hash structure from a target password-protected document (`My Locked PDF1.pdf`) using parser tools, formatting the string to start with `$pdf$`[span_24](start_span)[span_24](end_span)[span_25](start_span)[span_25](end_span).
3. **Execution:** Saved the target hash to a local text file (`hash1.txt`), loaded it into Johnny using the appropriate format profile, and initiated a dictionary-based attack[span_26](start_span)[span_26](end_span)[span_27](start_span)[span_27](end_span)[span_28](start_span)[span_28](end_span).
4. **Resolution:** Successfully matched and cracked the weak key (`password1`), granting decrypted access to the protected target file[span_29](start_span)[span_29](end_span)[span_30](start_span)[span_30](end_span).

### Module 2: Browser-Based Hash Extraction & Dictionary Analysis
1. **Local Processing:** Utilized client-side hash extraction modules to parse PDF metadata locally without exposing sensitive files[span_31](start_span)[span_31](end_span)[span_32](start_span)[span_32](end_span).
2. **Attack Simulation:** Deployed automated wordlist dictionaries against the extracted `$pdf$` hash string to measure time-to-crack metrics[span_33](start_span)[span_33](end_span).
3. **Validation:** Verified the recovered plaintext password against the document controls to confirm successful flag capture[span_34](start_span)[span_34](end_span)[span_35](start_span)[span_35](end_span).

---

## 🔒 Key Security Insights
* **The Danger of Weak Passwords:** Short or dictionary-based passwords (e.g., 8-character strings) can be brute-forced or dictionary-cracked in minutes[span_36](start_span)[span_36](end_span).
* **Encryption vs. Hashing:** Emphasized the structural difference between two-way encryption (reversible with a key) and one-way cryptographic hashing (requiring brute-force/dictionary iteration to reverse)[span_37](start_span)[span_37](end_span)[span_38](start_span)[span_38](end_span).
* **Defense-in-Depth:** Highlights the necessity of enforcing complex, long-form passwords and Multi-Factor Authentication (MFA) to mitigate credential compromise risks.
