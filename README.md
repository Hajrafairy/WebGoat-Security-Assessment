#  WebGoat Security Assessment

##  Project Overview
This project demonstrates penetration testing and security hardening using OWASP WebGoat.

---

## Tools Used

- Kali Linux
- Nmap
- Burp Suite
- Wireshark
- WebGoat
- NodeJS
- Winston (Logging)
- bcrypt (Password hashing)
- Helmet (Security headers)

---

##  Setup Instructions

### 1 Run WebGoat
Download and run:
java -jar webgoat-server-8.2.2.jar

Access:
http://localhost:8080/WebGoat

### 2️ Run Secure NodeJS App
cd secure-app
npm install
node server.js

---

##  Vulnerabilities Identified

### 1. Cross-Site Scripting (XSS)
Reflected XSS was successfully executed.

### 2. SQL Injection
Login bypass using ' OR '1'='1 was successful.

### 3. No HTTPS
Credentials transmitted in plaintext.

---

## Fixes Implemented

✔ Prepared statements to prevent SQL injection  
✔ Helmet for XSS protection  
✔ bcrypt for password hashing  
✔ Winston for logging  
✔ HTTPS enabled  

---

##  Screenshots

Screenshots are available inside the Screenshots folder.

---

##  Conclusion

The WebGoat application contains multiple OWASP Top 10 vulnerabilities.  
Security best practices were implemented to mitigate these risks.
