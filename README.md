# 🔐 Week 3 Project Modules: Password Cracking

## 📖 Overview
This repository contains the documentation and step-by-step walkthroughs for **Week 3 | Project Module 1** and **Project Module 2**. The labs focus on practical password security assessment by recovering the password of a protected PDF file using two methods:
1. **John the Ripper (JTR) & Johnny** for local desktop cracking.
2. **Networkwalks Hash Calculator & Password Cracker** for browser-based cracking.

## 🎯 Objective
Successfully crack the password of the attached protected document (`My Locked PDF1.pdf`) to understand the mechanics of password cracking and the necessity of strong password policies.

## 🛠️ Prerequisites
* **Operating System:** Windows PC (Kali Linux users have JTR pre-installed).
* **Target File:** `My Locked PDF1.pdf`.

---

## 🚀 Module 1: John the Ripper (JTR)

### Step 1: Environment Setup
1. Download the latest Jumbo release of John the Ripper for Windows from the [official Openwall website](https://www.openwall.com/john/).
2. Download the Johnny GUI from the [official Johnny page](https://openwall.info/wiki/john/johnny).
3. Run `johnnyInstaller.exe` and open Johnny.
4. Go to **Settings**, click **Browse**, and locate `john.exe` inside the `run` folder of your extracted JTR directory.

### Step 2: Hash Extraction
1. Navigate to the [Online Hash Crack - PDF Hash Extractor](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php).
2. Upload `My Locked PDF1.pdf`.
3. Copy the generated hash string.

## 🚀 Module 2: Networkwalks Tools

### Step 1: Hash Extraction
Open the Networkwalks Hash Calculator.   
Switch to the PDF tab and upload My Locked PDF1.pdf.   
Copy the full extracted hash starting strictly with $pdf$.   

### Step 2: Dictionary Attack
Open the Networkwalks Password Cracker.   
Paste your copied hash into the PDF HASH ($PDF$...) field.   
Ensure Built-in list (100 passwords) is active and click START CRACKING.   
The tool will match the hash against its dictionary and display the successful password (password1).   
Open the locked PDF and unlock it using the cracked password.   
