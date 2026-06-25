# FUTURE_CS_03
Read-only API security audit focusing on OWASP vulnerabilities like Excessive Data Exposure and Missing Rate Limiting.
# API Security Risk Analysis (SaaS Security) 🔐

## Objective
This repository contains a professional **API Security Risk Analysis Report** completed as part of the Cyber Security Internship at Future Interns. The goal of this project was to act as an AppSec Consultant to perform a read-only security audit on a public test API (`jsonplaceholder.typicode.com`), identifying critical architectural vulnerabilities.

## Scope & Methodology
* **Tools Used:** Postman, Browser DevTools.
* **Testing Scope:** Passive, read-only analysis (GET requests). Strict adherence to ethical hacking and API documentation guidelines.
* **Focus Areas:** Analyzed endpoints based on the OWASP API Security Top 10 framework.

## Key Findings Identified
1. **Unauthenticated Endpoint Access:** The API lacks API Key, JWT, or OAuth validation, allowing public access to sensitive endpoints.
2. **Excessive Data Exposure:** The backend returns complete database objects (including PII like phone numbers and exact GPS coordinates) instead of utilizing Data Transfer Objects (DTOs) to filter responses.
3. **Missing Rate Limiting:** Inspection of HTTP headers revealed an absence of API Gateway throttling, leaving the server vulnerable to automated scraping and Denial of Service (DoS) attacks.

## Deliverables
* **[API Security Risk Analysis Report (PDF)](link-to-your-pdf)** - Contains detailed risk classifications, business impact summaries, and technical remediation steps for backend developers. Includes Postman evidence.
