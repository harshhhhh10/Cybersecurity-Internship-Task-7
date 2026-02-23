# Research: How Malicious Browser Extensions Can Harm Users

## 1. Data Theft & Credential Stealing
Malicious extensions can silently read everything typed 
on websites including usernames, passwords, credit card 
numbers, and OTPs. Since many extensions have "read data 
on all websites" permission, they capture form inputs 
before data is even submitted.

**Real Example:** The DataSpii breach (2019) involved 
extensions like Hover Zoom and SpeakIt that collected 
and leaked browsing history of millions of users including 
sensitive URLs containing personal data, corporate 
documents, and medical records.

---

## 2. Session Hijacking & Cookie Theft
Extensions can access browser cookies including session 
cookies. With a session cookie, an attacker can log into 
accounts (Gmail, banking, social media) without knowing 
the password — no 2FA required since the session is 
already authenticated.

**How it works:**
1. User logs into bank → browser stores session cookie
2. Malicious extension reads and sends cookie to 
   attacker's server
3. Attacker uses cookie to access account from 
   their own device

---

## 3. Keylogging
Some malicious extensions inject JavaScript into every 
webpage visited and record every keystroke. This captures 
passwords even on HTTPS sites because the attack happens 
inside the browser after decryption.

---

## 4. Ad Injection & Click Fraud
Extensions can:
- Insert fake ads into legitimate websites
- Replace existing ads with their own (stealing ad revenue)
- Secretly click on ads in background to generate 
  fraudulent revenue
- Redirect searches to affiliated sites to earn commissions

**Real Example:** Superfish (2015) was pre-installed on 
Lenovo laptops and injected ads into search results, 
also breaking HTTPS security in the process.

---

## 5. Browser Hijacking
Malicious extensions can:
- Change default search engine to a fake/tracking one
- Redirect homepage to a phishing or ad-heavy site
- Intercept and modify web pages before the user sees them
- Block access to security websites like antivirus servers

---

## 6. Cryptojacking
Extensions can secretly use the CPU to mine cryptocurrency 
(like Monero) in the background without user knowledge.

**Effects:**
- Significantly slower browser and computer performance
- Higher electricity consumption
- Potential hardware damage from sustained overheating

**Real Example:** Archive Poster (2017) was found secretly 
mining cryptocurrency using browsers of its 105,000 users.

---

## 7. Phishing & Man-in-the-Browser (MitB) Attacks
Malicious extensions can modify banking websites in 
real time to:
- Add fake form fields to steal extra information
- Change recipient account number during online transfer
- Display fake "account locked" messages to steal credentials

This is extremely dangerous because the URL and SSL 
certificate still look completely legitimate to the user.

---

## 8. Spying & Surveillance
Extensions can:
- Track every website visited
- Record time spent on each page
- Monitor search queries
- Build and sell detailed behavioral profiles

**Real Example:** Several VPN and utility extensions 
were found selling user browsing data to third-party 
data brokers without clear disclosure.

---

## 9. Malware Distribution
Some extensions act as droppers — they download and 
install additional malware by exploiting browser or OS 
vulnerabilities. This can lead to ransomware, spyware, 
or full system compromise.

---

## 10. Supply Chain Attacks
Even legitimate, trusted extensions can become dangerous:
- Developer's account gets hacked → malicious update pushed
- Developer sells extension to malicious buyer
- A dependency the extension uses gets compromised

**Real Example:** The Great Suspender (2021) — a popular 
Chrome extension with 2M+ users was sold to unknown buyers 
who quietly added tracking code. Google eventually removed 
it from the Chrome Web Store.

---

## Attack Summary Table

| Attack Type | Method | Impact |
|---|---|---|
| Credential Theft | Captures typed passwords | Account takeover |
| Session Hijacking | Steals login cookies | Bypasses 2FA |
| Keylogging | Records all keystrokes | Exposes all sensitive input |
| Ad Injection | Inserts fake ads | Financial loss, privacy breach |
| Browser Hijacking | Changes search/homepage | Exposes user to phishing |
| Cryptojacking | Mines crypto secretly | Slow PC, high electricity bill |
| MitB Attack | Modifies banking pages in real time | Financial fraud |
| Surveillance | Tracks all browsing behavior | Privacy violation, data selling |
| Malware Dropping | Installs additional malware | Full system compromise |
| Supply Chain Attack | Compromises trusted extensions | Mass user infection |

---

## Protection Best Practices

| Practice | Why It Matters |
|---|---|
| Install only from official stores | Reduces risk of side-loaded malware |
| Check publisher identity | Unknown authors are a red flag |
| Read reviews before installing | Community often spots suspicious behavior |
| Audit permissions regularly | Permissions should match extension purpose |
| Keep extensions updated | Patches security vulnerabilities |
| Remove unused extensions | Reduces attack surface |
| Use extensions from reputable organizations | Accountable publishers |
| Monitor browser performance | Slowdowns can indicate cryptojacking |

---

## Conclusion
Browser extensions are powerful tools that operate with 
significant privileges inside the browser. While most 
extensions are legitimate and useful, malicious ones 
can cause serious harm ranging from credential theft 
to full system compromise. The key to staying safe is 
practicing careful evaluation before installation and 
regularly auditing installed extensions.
