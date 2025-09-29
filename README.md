# Kong Config Sync with GitHub Actions

This repository automates syncing Kong Gateway configuration with GitHub using [decK](https://github.com/kong/deck).

---

## 🚀 How it Works
- At **12 AM IST (18:30 UTC)** every day, GitHub Actions runs.
- The workflow uses **decK** to export Kong configuration (`deck dump`).
- The exported config is committed into this repository automatically.

---

## ⚙️ Setup Steps

### 1. Install decK (Optional: for local testing)
- **Mac**: `brew install deck`  
- **Linux**:  
  ```bash
  curl -sL https://github.com/kong/deck/releases/download/v1.43.0/deck_1.43.0_linux_amd64.tar.gz | tar xz -C /usr/local/bin
