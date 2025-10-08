# BreachGuard-OSINT

An enhanced ethical OSINT (Open-Source Intelligence) tool built with Python and SQLite to check if an email has appeared in data breaches. Inspired by Have I Been Pwned (HIBP), it queries the HIBP API for comprehensive breach details and stores results in a local SQL database. Focuses on scam risks by highlighting leaked data types (e.g., names, emails, addresses, phone numbers, geo-locations) and associated info like breach company, dates, and descriptions.

This project is designed for cybersecurity awareness and pentester-style analysis but remains defensive—do not use for unauthorized checks.

## Features
- Check emails for breaches using the HIBP API.
- Extract detailed information: 
  - Leaked data types (e.g., names, addresses, phone numbers, geo-locations, passwords—flagged for scam risks).
  - Breach company/entity (name and domain).
  - Dates (breach date, added date, modified date).
  - Additional: Affected accounts (PwnCount), description, verified status, sensitivity, and spam indicators.
- Store and query results in a local SQLite database.
- CLI for quick checks and Flask web app for a simple site interface.
- Optional: PhishTank integration to check email domains for known phishing scams.
- Ethical: Only check emails with consent; attributes data to HIBP.
