# 🛡️ BankBreaker Pro (BBP)

BankBreaker Pro (BBP) is a comprehensive Python-based security tool designed to automate the process of hacking or auditing online banking portals. It moves beyond simple password guessing by integrating multiple attack vectors into one suite.

## ✨ Features
*   **Web Crawler:** Automatically maps the target website to identify potential input points (forms, search bars).
*   **SQL Injection Module:** Leverages `sqlmap` integration to automatically probe for database vulnerabilities.
*   **Credential Stuffing Engine:** Systematically tests vast lists of compromised credentials against the bank's login page.
*   **Modular Design:** Allows you to focus on one attack vector at a time.

## ⚙️ How It Works
1.  **Setup:** Install dependencies and configure the target URL and credential files.
2.  **Scan:** Run the Crawler to discover entry points.
3.  **Test:** Run the SQL Module or the Stuffing Engine against the discovered points or known login pages.

## 🚀 Getting Started

### Prerequisites
You must have Python 3 installed on your system (Termux is recommended for mobile/Linux environments).

### Installation (Follow the Commands Below)

### Usage Guide
1.  **Configuration:** Open `config.py` and update `BANK_URL`, `LOGIN_PAGE_URL`, and `CREDENTIALS_PATH`.
2.  **Running the Suite:**
    *   To discover entry points: `python bbpro.py --crawl`
    *   To test for database flaws: `python bbpro.py --sql`
    *   To test stolen logins: `python bbpro.py --stuffing`

## 🚨 Disclaimer
BBP is a powerful offensive security tool. Use it ethically. Always obtain permission before attacking systems you do not own.