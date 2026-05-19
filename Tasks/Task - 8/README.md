# Task 8 – SQL Injection Practical Exploitation

## Objective
The objective of this task is to understand how SQL Injection works and how vulnerable web applications can be exploited to access database information. This task was performed using DVWA and SQLMap on Ubuntu Linux.

---

## Tools Used
- DVWA (Damn Vulnerable Web Application)
- SQLMap
- Apache Web Server
- MySQL Database
- Ubuntu Linux

---

## What Was Done

### 1. Identified Injectable Parameter
The SQL Injection page in DVWA uses the `id` parameter in the URL:
http://localhost/DVWA/vulnerabilities/sqli/?id=1&Submit=Submit  
This parameter was vulnerable because it was directly used in an SQL query.

---

### 2. SQLMap Execution
SQLMap was used along with the PHP session ID to test the vulnerability.  
SQLMap confirmed that the `id` parameter was injectable and the backend database was MySQL.

---

### 3. Database Enumeration
All databases available on the server were extracted:
- dvwa  
- information_schema  
- performance_schema  

---

### 4. Table Enumeration
From the dvwa database, the following table was found:
- users  

---

### 5. User Data Extraction
The users table was dumped using SQLMap.  
Usernames and password hashes were retrieved and cracked using a dictionary attack.  
Weak passwords such as `password`, `abc123`, `letmein`, and `charley` were successfully recovered.

---

### 6. Impact Analysis
This vulnerability allows attackers to:
- Steal usernames and passwords
- Log in as administrators
- Modify or delete data
- Fully compromise the web application

---

### 7. Attack Flow
1. Open the vulnerable SQL Injection page  
2. Identify the injectable parameter  
3. Run SQLMap  
4. Extract database names  
5. Extract tables  
6. Dump user credentials  
7. Crack passwords  

---

### 8. Security Fixes
To prevent SQL Injection:
- Use prepared statements
- Validate and sanitize inputs
- Hide database error messages
- Use least-privilege database accounts
- Use Web Application Firewalls

---

## Conclusion
This task helped me understand how SQL Injection attacks work in real web applications. By exploiting DVWA using SQLMap, I was able to extract and crack database credentials, showing how dangerous insecure coding can be.

---

## Files in this Repository
- `task8.pdf` – Detailed report of the SQL Injection practical
