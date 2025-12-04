# 🚀 AutoXSS-Detector  
### Advanced Automated XSS Scanner with GUI + Smart Reporting

Cross-Site Scripting (**XSS**) is a common and dangerous web vulnerability that allows attackers to inject malicious JavaScript into web pages viewed by others.  
It can lead to:

- Credential theft  
- Session hijacking  
- Phishing  
- Website defacement  
- Complete browser compromise  

Testing large batches of URLs manually for XSS is slow and repetitive — that’s where **AutoXSS-Detector** comes in.

---

# 🛡 What Is AutoXSS-Detector?

AutoXSS-Detector is a **GUI-based automated XSS scanning framework** that performs multi-threaded scanning using the xsscrapy engine.  
It loads URLs from a file, tests them in parallel, parses the scan results, removes duplicates, and generates a clean, structured final report.

Designed for:

- Bug bounty hunters  
- Web security analysts  
- Pentesters  
- Security automation workflows  

---

# ✨ Features

### 🔍 1. **Fully Automated XSS Scanning**
Load a `.txt` file of URLs → click **Start Scan** → everything runs automatically.

### ⚡ 2. **High-Speed Multi-Threading**
- Up to 20 parallel workers  
- Ideal for large URL lists  
- Timeout handling for slow URLs  

### 🧪 3. **Smart Result Extraction**
Parses xsscrapy output and extracts:

- Payload  
- URL  
- Response URL  
- Injection point  
- Possible payloads  
- Reflection confirmation  

### 🧹 4. **Automatic Duplicate Removal**
Automatically groups and removes duplicate findings using: Host + Path + Injection Point
Ensures **clean, unique** results.

### 📄 5. **Professional Final Report**
Generates: xss_final_report.txt
Including:
- Unique injection points  
- Full payload details  
- Summaries & statistics  

### 🎨 6. **Modern GUI**
- Dark cyberpunk theme  
- Live logs  
- Progress bars  
- Worker activity indicators  

### 🧩 7. **Auto Organizes Output**
Creates a timestamped folder:
xss_scan_results_YYYYMMDD_HHMMSS/
├── xss_final_report.txt
└── xsscrapy_outputs/

# 🔧 Workflow
```bash
┌──────────────────────────────────────────┐
│        1. Load URLs File (.txt)          │
└──────────────────────────┬───────────────┘
                           │
                           ▼
┌──────────────────────────────────────────┐
│        2. Start Scan (Multi-Thread)      │
│         Auto-launches xsscrapy           │
└──────────────────────────┬───────────────┘
                           │
                           ▼
┌──────────────────────────────────────────┐
│      3. Capture & Collect Results        │
│       (xsscrapy output files)            │
└──────────────────────────┬───────────────┘
                           │
                           ▼
┌──────────────────────────────────────────┐
│       4. Parse & Deduplicate Data        │
│    Extract: Payload, URL, response,      │
│       injection point + remove dups      │
└──────────────────────────┬───────────────┘
                           │
                           ▼
┌──────────────────────────────────────────┐
│         5. Generate Final Report         │
│       (Clean → xss_final_report.txt)     │
└──────────────────────────────────────────┘
```

# 💡 Why AutoXSS-Detector Is Unique

| Feature | AutoXSS-Detector | Typical Tools |
|--------|------------------|----------------|
| GUI interface | ✅ | ❌ |
| Multi-threading | ✅ Fast | ⚠ Slow |
| Deduplication engine | ✅ | ❌ |
| Auto final report | ✅ | ❌ |
| Organized output | ✅ | ❌ |
| Real-time logs | ✅ | ⚠ Minimal |

This tool is built specifically for **automation**, **speed**, and **clean reporting** — perfect for large-scale XSS analysis.
