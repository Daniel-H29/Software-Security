# CS-305 Project Two: Secure Software Development

## Reflection

**Client and Requirements**  
Artemis Financial is a financial consulting company specializing in personalized financial plans. They requested enhancements to their web application to improve secure communications, including implementing encryption, checksum verification, and vulnerability scanning to ensure client data protection.

**What Went Well**  
I successfully implemented HTTPS communication using a self-signed SSL certificate, integrated SHA-256 checksum verification for static data, and performed static security analysis using the OWASP Dependency-Check tool. Secure coding practices are critical to protect sensitive information, maintain client trust, and ensure compliance with regulations, all of which add significant value to the company's security posture.

**Challenges and Helpful Areas**  
Generating the SSL certificate and correctly configuring Spring Boot to enforce HTTPS were initially challenging. Using the OWASP Dependency-Check tool and learning how to suppress false positives improved my understanding of real-world DevSecOps practices.

**How I Increased Security Layers**  
I secured data transmission with HTTPS, validated data integrity using cryptographic hashing (SHA-256), and used static code analysis to detect and mitigate vulnerabilities in dependencies. This layered approach strengthened the application’s overall security.

**Verification After Refactoring**  
I tested the `/hash` endpoint over HTTPS, confirming that the server returned the correct SHA-256 checksum. I also reran the dependency check to verify that no new vulnerabilities were introduced after refactoring.

**Resources and Tools Used**  
- OWASP Dependency-Check Maven Plugin  
- Java Keytool for SSL certificate creation  
- SHA-256 hashing algorithm  
- Spring Boot security configuration

**Portfolio Artifact**  
I would present the Practices for Secure Software Report, the HTTPS-enabled application, and dependency-check reports as examples of my secure coding, DevSecOps practices, and secure communication implementation skills to future employers.
