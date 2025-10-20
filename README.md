# SNHU-CS305

Artemis Financial Secure Software Project Reflection
Client Summary
My client, Artemis Financial, is a financial consulting company that develops personalized savings, retirement, investment, and insurance plans for its clients. The company needed to modernize its software and strengthen its data security. Specifically, they wanted secure communication between their client web application and internal servers, along with a checksum verification feature to ensure data integrity during transfers.
Identifying and Addressing Vulnerabilities
I began by reviewing Artemis Financial’s existing code and identifying areas that lacked encryption or secure data validation. I added a secure cryptographic hash algorithm (SHA-256) for checksums and configured HTTPS communication using a self-signed SSL certificate. Coding securely is essential because it prevents data leaks, protects customer trust, and keeps businesses compliant with privacy regulations. Strong security practices improve a company’s reliability and reputation.
Challenges and Helpful Insights
The most challenging part was configuring the dependency-check tool and managing SSL certificates. However, it was also helpful because it showed how security tools interact with real-world systems and dependencies. I learned how encryption, hashing, and certificate management work together to ensure safe communication.
Increasing Layers of Security
I implemented multiple layers of protection: encrypted HTTPS communication, checksum verification for integrity, and secure key storage in a .p12 keystore. In the future, I would continue using static code analysis tools (like OWASP Dependency-Check or SonarQube) and perform penetration tests to identify potential weaknesses before deployment.
Ensuring Functionality and Security
After refactoring the code, I built and ran the application to confirm that it compiled and executed without errors. I then tested the /hash endpoint to verify that checksum values matched expected results and ran a dependency check to confirm that no new vulnerabilities were introduced. Functional testing confirmed the application’s integrity and secure performance.
Useful Tools and Practices
The most valuable tools and practices I used were the Java Keytool for certificate generation, Spring Boot for managing secure web endpoints, and OWASP Dependency-Check for vulnerability scanning. Understanding how to implement HTTPS and hash algorithms will be useful in any future software project that handles sensitive information.
Portfolio and Employer Value
For my portfolio, I chose to include the Artemis Financial Practices for Secure Software Report. This project demonstrates my ability to assess vulnerabilities, refactor code securely, and implement modern encryption standards. I can show future employers my understanding of applied cybersecurity principles, from encryption and authentication to secure deployment and testing.
