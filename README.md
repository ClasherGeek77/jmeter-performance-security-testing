# jMeter-Owasp-Example 🛡️

[![Performance](https://img.shields.io/badge/Performance-JMeter-red?logo=apachejmeter)]()
[![Security](https://img.shields.io/badge/Security-OWASP%20ZAP-blue?logo=owasp)]()

A cohesive demonstration repository illustrating how QA Engineers can bridge the gap beyond functional automation into **Performance Load Testing** and basic **Dynamic Application Security Testing (DAST)**.

## 🎯 Objective
To provide foundational workflows for stress-testing REST APIs and automating security vulnerability scans natively in CI/CD.

## 🏗 Architecture & Technologies
- **Load Generation**: Apache JMeter (JMX files configured for Thread Groups, Timers, and Listeners).
- **Security Scanning**: OWASP ZAP (Zed Attack Proxy) running via Docker natively.

## ⚙️ Key Technical Highlights
1. **CLI Execution**: Bypassing JMeter GUI for highly efficient CLI load execution.
2. **HTML Dashboard Generation**: Extracting JMeter `.jtl` files into robust visual dashboards.
3. **ZAP Baseline Scans**: Automatically spidering external endpoints to detect unencrypted transmissions, missing security headers, and common injection vulnerabilities.

## 🚀 Getting Started
```bash
# Example JMeter Headless Execution
jmeter -n -t Scripts/API_Load.jmx -l results.jtl -e -o /Reports/
```

> *"I don't just automate tests. I build testers."* — Teddy Lioner
