# Task 7 – Web Application Vulnerability Testing

This project demonstrates web application security testing using DVWA (Damn Vulnerable Web Application) and Burp Suite Community Edition.

## Tools Used
- Burp Suite Community Edition
- DVWA (Damn Vulnerable Web Application)

## Vulnerabilities Tested
- SQL Injection
- Reflected Cross-Site Scripting (XSS)

## What I Did
I installed DVWA on my local system and set the security level to Low.  
I configured Burp Suite as a proxy and used its built-in browser to access DVWA.

Using Burp’s HTTP History, I intercepted and analyzed:
- SQL Injection requests  
- XSS requests  

I verified vulnerabilities by injecting payloads and observing the application responses.

## Evidence
The Burp HTTP History shows traffic for:
- /DVWA/vulnerabilities/sqli/
- /DVWA/vulnerabilities/xss_r/

These confirm that SQL Injection and XSS were successfully tested.

## Conclusion
This lab helped me understand how real attackers exploit insecure web applications and how Burp Suite is used by security professionals to detect such issues.
