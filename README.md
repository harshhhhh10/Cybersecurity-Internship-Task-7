# Task 7: Identify and Remove Suspicious Browser Extensions

## Objective
Learn to spot and remove potentially harmful browser extensions
using Firefox's Add-ons Manager.

## Browser Used
Mozilla Firefox

## Tools Used
- Mozilla Firefox Browser
- Firefox Add-ons Manager (about:addons)
- addons.mozilla.org for publisher verification

---

## Step-by-Step Process

### Step 1: Opened Firefox Add-ons Manager
Navigated to `about:addons` in Firefox to access the 
Extensions manager.

📸 Screenshot: `screenshots/screenshot1_all_extensions.png`

### Step 2: Installed Extensions for Audit
Installed 3 extensions to perform a security audit:
- uBlock Origin
- Privacy Badger
- HTTPS Everywhere Lite+

### Step 3: Reviewed Permissions of Each Extension
Clicked on each extension → Permissions and data tab 
to review what access each extension requested.

📸 Screenshot: `screenshots/screenshot2_ublockorigin_permissions.png`
📸 Screenshot: `screenshots/screenshot3_privacybadger_permissions.png`
📸 Screenshot: `screenshots/screenshot4_httpslite_permissions.png`

### Step 4: Identified Suspicious Extension
Flagged HTTPS Everywhere Lite+ as suspicious based on 
multiple red flags (see table below).

### Step 5: Removed Suspicious Extension
Clicked ··· → Remove → Confirmed removal of 
HTTPS Everywhere Lite+. Also had the option to 
"Report this extension to Mozilla" during removal.

📸 Screenshot: `screenshots/screenshot5_removal_popup.png`

### Step 6: Verified Clean State
Confirmed only trusted extensions remain installed.

📸 Screenshot: `screenshots/screenshot6_final_clean.png`

---

## Extensions Reviewed

| Extension | Publisher | Permissions | Red Flags | Verdict |
|---|---|---|---|---|
| uBlock Origin | Raymond Hill (gorhill) | Access all website data, read/modify privacy settings, access browser tabs, access browser activity during navigation. No data collection. | None — open source, millions of users, verified by Mozilla | ✅ Safe — Kept |
| Privacy Badger | EFF (Electronic Frontier Foundation) | Access all website data, read/modify privacy settings, access browser tabs, access browser activity during navigation | None — made by reputable non-profit EFF, verified by Mozilla | ✅ Safe — Kept |
| HTTPS Everywhere Lite+ | Enia Onec | Access your data for all websites | Unknown publisher, 0 reviews, unofficial fork of discontinued EFF tool, no Mozilla verification badge | ⚠️ Suspicious — Removed |

---

## Suspicious Extension Found & Removed

### HTTPS Everywhere Lite+
**Reason for Flagging:**
- **Unknown Publisher:** Author listed as "Enia Onec" — 
  no verifiable identity, organization, or track record
- **Zero Reviews:** 0 ratings on Firefox Add-ons store — 
  no community trust or verification whatsoever
- **Unofficial Fork:** The original HTTPS Everywhere by EFF 
  was officially discontinued; this is an unverified community 
  replacement claiming to do the same job
- **No Trust Badges:** Unlike uBlock Origin and Privacy Badger, 
  it had no Recommended or Verified badges from Mozilla
- **Very Low Version:** Version 1.3 with no established history

**Action Taken:** Extension removed via Firefox Add-ons Manager.
**Reported:** Firefox offered option to report to Mozilla 
during removal process.

---

## Key Learning

> Fewer permissions do not automatically mean an extension 
> is safe. Publisher credibility, review count, and origin 
> matter just as much as the permissions list.

A legitimate extension from a trusted publisher with broad 
permissions (like uBlock Origin) is safer than an obscure 
extension with minimal permissions from an unknown author 
with zero reviews.

---

## Interview Questions 

**1. How can browser extensions pose security risks?**
Extensions run with elevated browser privileges and can 
access webpage content, steal login credentials, inject ads, 
track browsing history, hijack sessions, or redirect traffic 
to malicious sites. They can also act as droppers to install 
additional malware.

**2. What permissions should raise suspicion?**
The most dangerous permissions include:
- "Read and change all your data on all websites"
- Access to clipboard
- Download management
- Browsing history access
- Access to tabs and navigation activity

These are especially suspicious when requested by an 
unknown publisher with few or no reviews.

**3. How to safely install browser extensions?**
- Only install from official stores (Firefox Add-ons / 
  Chrome Web Store)
- Verify the publisher's identity and reputation
- Check user reviews and star ratings
- Review permissions before installing
- Look for Mozilla Recommended or Verified badges
- Research the extension name online if unsure

**4. What is extension sandboxing?**
Extension sandboxing is a security mechanism that isolates 
extensions from each other and from the operating system. 
It means a compromised extension cannot directly access 
other browser processes, system files, or other extensions' 
data. However, sandboxing does not prevent extensions from 
accessing web page content they have permission for.

**5. Can extensions steal passwords?**
Yes. Extensions with "read all website data" permissions 
can capture form inputs including passwords typed on any 
website. This happens inside the browser after HTTPS 
decryption, so even secure sites are vulnerable. Some 
extensions also perform keylogging by injecting JavaScript 
into every page visited.

**6. How to update extensions securely?**
Enable automatic updates in browser settings. In Firefox, 
this is configurable per extension under:
Details > Allow automatic updates > Default (Recommended)
Only install updates from the official add-on store, 
never from pop-ups or external websites.

**7. Difference between extensions and plugins?**
Extensions add features to the browser UI and interact 
with web pages using standard web technologies (HTML, CSS, 
JavaScript). They are sandboxed within the browser.
Plugins (like Adobe Flash, now deprecated) ran native 
compiled code outside the browser's normal environment 
to handle specific content types and had much deeper 
system access, making them a bigger security risk.

**8. How to report malicious extensions?**
- In Firefox: Visit the extension's page on 
  addons.mozilla.org → scroll down → click 
  "Report this add-on for abuse"
- During removal: Firefox shows a checkbox 
  "Report this extension to Mozilla"
- In Chrome: Open Chrome Web Store page of the 
  extension → scroll down → "Report abuse"
- You can also report to your organization's 
  IT/security team if on a managed device

---

## Research
See [research.md](./research.md) for detailed analysis 
of how malicious browser extensions can harm users,
including real-world examples.

---

## Outcome
Successfully identified and removed one suspicious extension 
(HTTPS Everywhere Lite+) based on unknown publisher, zero 
reviews, no Mozilla verification, and unverified origin. 
Retained two trusted security extensions from reputable 
publishers (EFF and Raymond Hill).

Gained hands-on understanding of:
- How to audit browser extensions
- What red flags to look for
- How to evaluate permissions in context
- How to safely remove and report suspicious extensions
