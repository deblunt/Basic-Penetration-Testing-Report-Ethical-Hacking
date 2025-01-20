# TechEcommerce Project - Penetration Testing Report


__Group Members :__ <br><br>

[Faisal Ahmed](https://github.com/FaisalAhmed21) | [MD. Shafiur Rahman](https://github.com/ShafiurShuvo) | [MD. Nafizur Rahman Bhuiya]() | [Maisa Tarannum Srizee]() | [Naima Nawar Achol]()


## Overview
This repository contains the penetration testing report for the **TechEcommerce Project**, performed by the **Zero Day Defenders** group as part of the Ethical Hacking course (CSE496, Fall 2024). The project focused on identifying vulnerabilities, testing exploit scenarios, and providing recommendations to secure the application.

---

## Project Setup
- Installed XAMPP and set up the project in the `htdocs` folder.
- Manually recreated the database due to missing `.sql` files.

---

## Attack Summary
### Successful Attacks
1. **SQL Injection**: Bypassed authentication; fixed with prepared statements.
2. **Data Tampering**: Altered sensitive data; fixed with validation and encryption.
3. **Replay Attack**: Reused requests; mitigated with nonces and token validation.
4. **Brute Force**: Exploited weak credentials; added rate limiting and CAPTCHA.
5. **Data Disclosure**: Accessed sensitive data; secured with encryption and access controls.
6. **IDOR**: Manipulated resources; resolved with proper authorization checks.

### Unsuccessful Attacks
1. **MITM**: Failed due to localhost constraints.
2. **Key Disclosure**: No encryption implemented.
3. **Tampered Content**: No upload features available.
4. **CSRF**: Cross-origin requests not supported.
5. **XSS**: No dynamic input to exploit.

---

## Fixes Implemented
- **Prepared Statements for SQL Queries**: Implemented using `mysqli_stmt_bind_param()` to ensure input sanitization and prevent SQL injection.
- **Password Hashing**: Passwords are hashed using `password_hash()` with the `PASSWORD_BCRYPT` algorithm for enhanced security.

---

## Recommended Fixes (Pending Implementation)
- **AES-256 Encryption**: Recommended for securing data at rest.
- **Role-Based Access Control (RBAC)**: Suggested for enforcing least privilege access.
- **Nonces and Tokens**: Advised for validating requests to mitigate replay attacks.
- **Detailed Logging**: Proposed for anomaly detection and tracking unauthorized access attempts.

---

## Conclusion
The project identified and resolved critical vulnerabilities, enhancing application security. Unsuccessful attacks highlighted additional preventive measures for real-world scenarios. Regular audits are recommended to maintain security.

For more details, visit the [repository](https://github.com/BrownBatsy/techEcommerce_project).
