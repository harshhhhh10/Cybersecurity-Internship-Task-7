# 🧩 Task 7 – Identify & Remove Suspicious Browser Extensions

![Internship](https://img.shields.io/badge/Elevate%20Labs-Cybersecurity%20Internship-blue?style=for-the-badge)
![Browser](https://img.shields.io/badge/Browser-Chrome%20%2F%20Edge-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)
![Topic](https://img.shields.io/badge/Topic-Browser%20Security-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

## 📌 Objective

Review installed browser extensions, identify suspicious or potentially harmful ones based on permissions and behavior, and remove any that pose a privacy or security risk.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Chrome / Edge Extensions Manager** | Review installed extensions |
| **Chrome Web Store** | Verify extension legitimacy |
| **Manual permission audit** | Identify over-privileged extensions |

---

## 🔍 What Makes an Extension Suspicious?

| Red Flag | Why It's Dangerous |
|----------|--------------------|
| Requests "Read all site data" | Can steal passwords, banking info, cookies |
| Unknown publisher | No accountability if it turns malware |
| Very few reviews / low rating | Not vetted by the community |
| Requests more permissions than needed | Over-privileged = higher risk |
| Not updated in years | May have unpatched vulnerabilities |
| Installed without your knowledge | Classic sign of adware/malware |

---

## 🧪 Audit Process

### Step 1 — Open Extensions Manager
```
Chrome: chrome://extensions
Edge:   edge://extensions
```

### Step 2 — Review Each Extension
For every installed extension, check:
- ✅ Do you recognize it?
- ✅ Is the publisher verified?
- ✅ Are the permissions reasonable for what it does?
- ✅ Does it have good reviews on the Web Store?

### Step 3 — Check Permissions Detail
Click **Details** → **View permissions** for each extension to see exactly what it can access.

### Step 4 — Remove Suspicious Extensions
Click **Remove** on any extension that fails the audit.

### Step 5 — Verify Browser Behavior After Removal
Confirm no unwanted redirects, pop-ups, or homepage changes remain.

---

## ⚠️ Common Malicious Extension Behaviors

- **Ad injection** — Inserts ads into websites you visit
- **Search hijacking** — Changes your default search engine
- **Cookie theft** — Steals session cookies to hijack accounts
- **Keylogging** — Records keystrokes including passwords
- **Data exfiltration** — Sends your browsing history to third parties
- **Cryptojacking** — Uses your CPU to mine cryptocurrency in the background

---

## 🛡️ Best Practices for Browser Extension Safety

1. **Install only from official stores** — Chrome Web Store / Firefox Add-ons
2. **Check permissions before installing** — Does a calculator need "read all site data"?
3. **Prefer extensions with large review counts** — Community-vetted is safer
4. **Keep extensions updated** — Updates patch security vulnerabilities
5. **Remove extensions you no longer use** — Reduce attack surface
6. **Audit extensions periodically** — Monthly review is good practice
7. **Use a dedicated browser profile** — Isolate sensitive browsing (banking, etc.)

---

## 📸 Screenshots

All screenshots are in the [`/screenshots`](./screenshots) folder:

| File | Description |
|------|-------------|
| `01_extensions_list.png` | Full list of installed extensions |
| `02_permissions_review.png` | Permission details of an extension |
| `03_suspicious_extension.png` | Flagged suspicious extension |
| `04_extension_removed.png` | After removal confirmation |

---

## 🧠 Key Learnings

- How browser extensions can be used as attack vectors
- How to audit extension permissions effectively
- What over-privileged extensions can access
- How to identify signs of adware and malicious extensions
- Importance of regular browser security hygiene

---

## 📁 Repository Structure

```
Cybersecurity-Internship-Task-7/
├── README.md
└── screenshots/
    ├── 01_extensions_list.png
    ├── 02_permissions_review.png
    ├── 03_suspicious_extension.png
    └── 04_extension_removed.png
```

---

> 🔒 *This audit was performed on a personal browser for educational purposes only as part of the Elevate Labs Cybersecurity Internship.*
