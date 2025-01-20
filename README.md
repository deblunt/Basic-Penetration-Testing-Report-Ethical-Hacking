# TechEcommerce Project - Penetration Testing Report<br><br>


## Group Members:  <br><br>

[Faisal Ahmed](https://github.com/FaisalAhmed21) | [MD. Shafiur Rahman](https://github.com/ShafiurShuvo) | [MD. Nafizur Rahman Bhuiya]() | [Maisa Tarannum Srizee]() | [Naima Nawar Achol]()<br><br>


## Overview <br><br>

This repository contains the penetration testing report for the **TechEcommerce Project**, performed by the **Zero Day Defenders** group as part of the Ethical Hacking course (CSE496, Fall 2024). The project focused on identifying vulnerabilities, testing exploit scenarios, and providing recommendations to secure the application.

---

## Project Setup  <br><br>

- Installed XAMPP and set up the project in the `htdocs` folder.
- Manually recreated the database due to missing `.sql` files.

---

## Attack Summary <br><br>

### Successful Attacks  <br><br>

1. **SQL Injection**
2. **Data Tampering**
3. **Replay Attack**
4. **Brute Force**
5. **Data Disclosure**
6. **Insider Attack**
7. **IDOR**

### Unsuccessful Attacks  <br><br>

1. **MITM**
2. **Key Disclosure**
3. **Tampered Content**
4. **CSRF**
5. **XSS**

---

## Fixes Implemented  <br><br>

- **Prepared Statements for SQL Queries**
- **Password Hashing**

---

## Recommended Fixes (Pending Implementation)  <br><br>

- **AES-256 Encryption**
- **Role-Based Access Control (RBAC)**
- **Nonces and Tokens**
- **Detailed Logging**

---

## Conclusion <br><br>

The project identified and resolved critical vulnerabilities, enhancing application security. Unsuccessful attacks highlighted additional preventive measures for real-world scenarios. Regular audits are recommended to maintain security.

For more details, visit the [repository](https://github.com/BrownBatsy/techEcommerce_project).
