Web Application Security 
Overview

This project demonstrates practical web application security testing using WebGoat and OWASP ZAP. The objective was to identify and exploit common vulnerabilities such as SQL Injection, Cross-Site Scripting (XSS), and Cross-Site Request Forgery (CSRF).

Objectives
Understand common web vulnerabilities
Perform automated and manual security testing
Exploit vulnerabilities in a controlled environment
Recommend mitigation strategies

Tools Used
WebGoat (vulnerable web application)
OWASP ZAP (security scanner)
Kali Linux

Setup
1. Run WebGoat
java -jar webgoat-server-8.2.2.jar
Access:
http://localhost:8080/WebGoat

2. Launch OWASP ZAP
zaproxy
Use Manual Explore or Automated Scan
Target:
http://localhost:8080/WebGoat

 Vulnerabilities Identified

 Cross-Site Scripting (XSS)

Payload:

<script>alert('XSS')</script>
Executes JavaScript in browser
Can steal cookies (document.cookie)

Mitigation:

Input validation
Output encoding
Content Security Policy (CSP)
Cross-Site Request Forgery (CSRF)
Tricks users into unintended actions

Mitigation:

Use CSRF tokens
Validate request origin

ZAP Analysis
Active scan performed
Vulnerabilities identified via the Alerts tab
Traffic captured in the Sites panel


Key Learnings
Importance of secure coding practices
Real-world impact of web vulnerabilities
Hands-on experience with security tools
