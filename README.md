# 🧩 Browser Extension Security Audit and Performance Analysis

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Repo Status](https://img.shields.io/badge/Status-Lab%20Report-brightgreen)]()

---

## 📝 Overview

This repository documents a practical cybersecurity exercise aimed at analyzing and securing a web browser environment by auditing installed extensions.  
The objective was to identify suspicious add-ons, review their permissions, assess security risks, and measure performance impact before and after cleanup.

---

## 🌐 Environment Details

- **Browser:** Google Chrome  
- **Operating System:** Windows 11 
- **Total Extensions Reviewed:** 10  
- **Extensions Removed:** 6  
- **Extensions Retained:** 4  

---

## 🧪 Lab Exercise: Methodology & Phases

### **Phase 1 — Preparation and Extension Discovery**

- Opened Chrome’s Extension Manager via `chrome://extensions/`.  
- Listed all currently installed browser extensions.  
- Verified each extension’s developer, permissions, and functionality through Chrome Web Store details and user reviews.  

**Initial List of Installed Extensions:**  
AdGuard, Shimeji, Wappalyzer, NodeFlair, Always Active Windows, Allow Copy, QuillBot, Volume Master, Google Translator, ChatGPT.  

---

### **Phase 2 — Evaluation of Permissions and Legitimacy**

- Reviewed each extension’s permission scope.  
- Classified them into three categories: **Safe**, **Moderate Risk**, and **Suspicious**.  
- Focused on identifying:
  - Overly broad permissions (e.g., “Read and change all your data on all websites”).  
  - Low or fake user ratings.  
  - Unknown publishers or limited documentation.  

**Key Findings:**  
Extensions like *Allow Copy*, *Always Active Windows*, and *ChatGPT (unofficial)* requested high-level privileges that could manipulate webpage content or collect browsing data.

---

### **Phase 3 — Removal of Suspicious or Unnecessary Extensions**

The following extensions were **removed** due to potential privacy, performance, or security risks:

| Extension Name | Reason for Removal |
|----------------|--------------------|
| Shimeji | Non-essential; high memory use |
| NodeFlair | Unverified developer; unclear permissions |
| Always Active Windows | Script injection and tab control risk |
| Allow Copy | JavaScript injection; privacy concerns |
| Volume Master | Duplicated versions known to be malicious |
| ChatGPT (Unofficial) | Multiple fake copies with data theft history |

**Retained (Safe) Extensions:**  
AdGuard, Wappalyzer, QuillBot (official), and Google Translator.  

---

### **Phase 4 — Browser Restart and Performance Assessment**

After cleaning the environment, the browser was restarted to assess resource consumption and responsiveness.

| Observation Metric | Before Cleanup | After Cleanup |
|--------------------|----------------|----------------|
| Startup Time | ~4 seconds | ~2 seconds |
| Memory Usage | 1.2 GB | 950 MB |
| CPU Utilization | Moderate | Noticeably reduced |
| Tab Load Time | 3–4 sec average | 1–2 sec average |
| Pop-ups / Lags | Occasional | None observed |

**Result:**  
Browser startup and tab-switching speed improved significantly. No background processes or pop-ups were detected post-cleanup.

---

### **Phase 5 — Security Impact Analysis**

Post-audit research revealed that malicious browser extensions can:

- Steal cookies, passwords, or clipboard data.  
- Inject phishing scripts or unwanted advertisements.  
- Redirect traffic to fake or malicious websites.  
- Track browsing patterns and collect sensitive analytics data.  

**Case Studies:**
- *DataSpii Breach* — Chrome extensions secretly collected user data from over 4 million users.  
- *Fake AdBlock Plus Incident* — Malicious clone installed by over 37,000 users before being removed.  

---

### **Phase 6 — Summary of Findings and Interpretation**

**1. Security Findings**  
- Six extensions had unnecessary or dangerous permissions.  
- Four official and verified extensions were retained.  
- Browser’s overall security posture improved after cleanup.  

**2. Performance Findings**  
- Memory usage decreased by ~20%.  
- Startup and browsing speeds improved notably.  

**3. Overall Conclusion**  
The browser extension audit reinforced the importance of periodic checks and removing unverified add-ons.  
Maintaining only trusted, essential extensions ensures better performance and reduced exposure to malicious activity.  

---

## ✅ Recommendations

- Install extensions **only from official web stores** and verified developers.  
- **Review permissions** before installation — avoid extensions needing full data access.  
- Perform **extension audits monthly or quarterly**.  
- Keep the browser **updated** to minimize exploit risks.  
- Use an **ad-blocker and antivirus** for an additional layer of defense.  

---

## 📁 Files & Artifacts (Lab)
- `BROWSER_EXTENSION_AUDIT.md` — This document.  
- `before_cleanup_screenshot.png` — Initial extension list.  
- `after_cleanup_screenshot.png` — Cleaned browser extension list.  
- `performance_table.csv` — Optional recorded metrics before and after cleanup.  


All actions were performed on a **personal system** without any unauthorized access or data manipulation.

---

## License
This work is licensed under the [MIT License](https://opensource.org/licenses/MIT).
