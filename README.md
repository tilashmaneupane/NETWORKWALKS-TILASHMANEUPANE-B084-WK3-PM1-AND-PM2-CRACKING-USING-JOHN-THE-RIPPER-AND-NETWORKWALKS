# Project Module 1: Password Cracking with John the Ripper (JTR)

## 📖 Overview
This repository contains the documentation and step-by-step walkthrough for **Week 3 | Project Module 1**. The lab focuses on practical password security assessment by recovering the password of a protected PDF file using John the Ripper (JTR) and its graphical interface, Johnny.

> **Note:** This documentation is directly based on the reference file: `W3-PM1 - Week3 - Project Module1 - Password Cracking with JTR v1.pdf`.

## 🎯 Objective
Successfully crack the password of the attached protected document (`My Locked PDF1.pdf`) on a Windows environment to understand the mechanics of password cracking and the necessity of strong password policies.

## 🛠️ Prerequisites
Before you begin, ensure you have the following:
* **Operating System:** Windows PC (Note: Kali Linux users have JTR pre-installed natively).
* **Target File:** `My Locked PDF1.pdf`
* **John the Ripper (JTR):** Open-source password security auditing tool.
* **Johnny GUI:** A graphical front-end for JTR.

## 🚀 Step-by-Step Walkthrough

### Step 1: Environment Setup

1. **Download JTR:** Fetch the latest Jumbo release of John the Ripper for Windows from the [Official Openwall Website](https://www.openwall.com/john/).
2. **Extract JTR:** Unzip the downloaded file to an easily accessible directory (e.g., `Downloads\JTR_John CLI Win x64`).
3. **Download Johnny GUI:** Get the Johnny GUI from the [Official Johnny Page](https://openwall.info/wiki/john/johnny).
4. **Install and Link:**
   * Run `johnnyInstaller.exe`.
   * Open Johnny, go to the **Settings** tab.
   * Click **Browse** and locate the `john.exe` executable inside the `run` folder of your extracted JTR directory.

### Step 2: Hash Extraction

JTR cannot directly attack a PDF; it needs the file's hash representation.

1. Navigate to the [Online Hash Crack - PDF Hash Extractor](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php).
2. Click **Browse**, select `My Locked PDF1.pdf`, and click **Upload**.
3. Once processed, carefully copy the generated hash string. 
