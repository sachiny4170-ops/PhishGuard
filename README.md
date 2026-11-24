# PhishGuard — Hackathon Edition

A responsive phishing-awareness and triage demo built with HTML, CSS and vanilla JavaScript.

## Run locally
1. Extract the ZIP.
2. Open `index.html` in a modern browser, or use VS Code Live Server.
3. Navigate through Overview, URL Analyzer, Email Analyzer, Learning Center, Knowledge Check and Reports.

No installation, backend or API key is required.

## Working features
- URL structure and heuristic risk-indicator analysis. The submitted destination is **not opened**.
- Email subject/body pattern analysis. No message is sent or uploaded.
- Six short awareness modules.
- Five-question knowledge check with score and feedback.
- Session history, JSON report export and print summary.
- Responsive layout for desktop and mobile.

## Important technical scope
This is a client-side educational prototype. The URL and email checks are heuristic indicators, not a reputation verdict. It does not perform DNS resolution, TLS inspection, redirect tracing, malware analysis, attachment scanning, SPF/DKIM/DMARC validation, or external threat-intelligence lookups. A LOW result does not mean safe, and a HIGH result does not prove maliciousness.

For a production/hackathon deployment, consider adding:
- A backend API with input validation, rate limiting and audit logging.
- A trusted URL reputation provider (for example, an approved commercial or public threat-intelligence API), with API keys kept server-side.
- Email-header parsing for SPF/DKIM/DMARC results from authorized mail samples.
- Role-based analyst/admin accounts, database persistence, and organization-specific reporting.
- Privacy notice, retention controls, abuse protections and security testing.

## Demo safety
Use only public test strings or content you are authorized to analyze. Do not paste passwords, OTPs, recovery codes, private email content or confidential company data. Do not use this tool to test systems without permission.
