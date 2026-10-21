# TDT4237 Software Security

[← All courses](../readme.md)

[![Cryptography](https://img.shields.io/badge/Cryptography-1B5E20?style=for-the-badge&logoColor=white)](https://www.ntnu.edu/studies/courses/TDT4237)
[![Web Security](https://img.shields.io/badge/Web%20Security-CC0000?style=for-the-badge&logoColor=white)](https://www.ntnu.edu/studies/courses/TDT4237)
[![OWASP](https://img.shields.io/badge/OWASP-000000?style=for-the-badge&logo=owasp&logoColor=white)](https://en.wikipedia.org/wiki/OWASP)
[![CVSS](https://img.shields.io/badge/CVSS-8B0000?style=for-the-badge&logo=cve&logoColor=white)](https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System)
[![GDPR](https://img.shields.io/badge/GDPR-003399?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation)

Quizzes for the NTNU course TDT4237 Software Security and Data Protection, in three series: cryptography fundamentals, secure software development, and web application security.

## Contents

- [Cryptography fundamentals](#cryptography-fundamentals)
- [Software security](#software-security)
- [Web application security](#web-application-security)

## Cryptography fundamentals

A concise introduction to secure communication and encryption techniques.

**Quiz:** [Cryptography Basics](https://dev-quizmachine.itautomasjon.no/Quiz/Take/Cryptography1)

**Topics:** Block ciphers · Rounds in ciphers · HMAC · Message authentication · Elliptic Curve Cryptography · Public-key efficiency · Certification Authorities · Trust models · Public keys · Private keys · Authentication · Encryption · Security models · Cryptographic evaluation · Cryptographic techniques · Data protection

[↑ Back to top](#tdt4237-software-security)

## Software security

A series on secure development practices and application-level security.

### Software Security – Part 1

**Quiz:** [Software Security – Part 1](https://dev-quizmachine.itautomasjon.no/Quiz/Take/SoftwareSecurityPart1)

**Topics:** Recommended secure coding practices · Symmetric encryption use in secure transmission · Asymmetric encryption (public/private keys) · CVE vs CVSS purposes · Good security requirements · CIA Triad (Confidentiality, Integrity, Availability) · ROI of countermeasures after a data breach · Defenses against session hijacking · Buffer overflow defenses · Symmetric vs asymmetric encryption disadvantages · Django password validator implementation · Weaknesses of password authentication & improvements · Psychological factors in social engineering · Malicious AI attacks on recognition systems · Salt & pepper in cryptography (hashing) · Conditions when salt fails

### Software Security – Part 2

**Quiz:** [Software Security – Part 2](https://dev-quizmachine.itautomasjon.no/Quiz/Take/SoftwareSecurityPart2)

**Topics:** Buffer overflow in C code · Secure coding practices (captchas, defenses) · Command injection attack · False cryptography statements · Key generation best practices · Threat agent characteristics · String concatenation vulnerability · XML external entity (XXE) risk · Storing passwords securely (hashing, salting) · Other sensitive data exposure vulnerabilities · CVSS scoring metrics (Heartbleed case) · Token exploitation and protection · Insecure logging configuration · Secure logging and monitoring · One-Time Pad encryption & properties · OTP key reuse vulnerabilities · Biba vs Bell-LaPadula models · Penetration testing and applications · PoisonGPT attack steps · DevOps software deployment attack steps · Risk analysis threat dimensions · Zero-day exploit description

### Software Security – Part 3

**Quiz:** [Software Security – Part 3](https://dev-quizmachine.itautomasjon.no/Quiz/Take/SoftwareSecurityPart3)

**Topics:** SQL injection vulnerability in Django code · Secure coding fix for raw SQL · Recommended secure practices · CIA triad violation · Password policy exceptions · Sensitive information exposure vulnerabilities · Vulnerability prioritization (CVSS scoring) · Common Vulnerability Scoring System (CVSS) · Common Vulnerabilities and Exposures (CVE) · Importance of updating NuGet packages · Insecure web parameters (URL issues) · CVE vs CVSS purposes · Asymmetric key usage · Backdoors in software · Countermeasure cost vs asset value · Phishing/email scam defense · Taboo traps in machine learning · Lawful consent under GDPR · Logic bomb attack · Unicode sabotage in translation systems · Password policy enforcement in Django · Secure logging and monitoring configuration

### Software Security – Part 4

**Quiz:** [Software Security – Part 4](https://dev-quizmachine.itautomasjon.no/Quiz/Take/SoftwareSecurityPart4)

**Topics:** GDPR L-F-D-A-S-I-A fields · Business goals and business assets · Business risks and risk dimensions · Misuse case diagram and threat agent ranking · Attack tree for QR code misuse · Technical risks linked to business risks · Security requirements for technical risks · GDPR violation discussion in crisis contexts · Machine learning use and misuse in identity · GDPR principles (Art. 5) · GDPR key points and legal bases · GDPR breach notification requirements

### Software Security – Part 5

**Quiz:** [Software Security – Part 5](https://dev-quizmachine.itautomasjon.no/Quiz/Take/SoftwareSecurityPart5)

**Topics:** STRIDE threat categories · Rule-Set-Based Access Control (RSBAC) · Organization-Based Access Control · Lattice-Based Access Control (LBAC) · Graph-Based Access Control (GBAC) · Context-Based Access Control (CBAC) · Bell-LaPadula model · Biba model · Clark-Wilson model · Brewer-Nash (Cinderella) model · Password salting defenses · Security by Design principles · Bell-LaPadula vs Biba differences · Bell-LaPadula vs Biba similarities · Secure coding practices · Security testing and code review · Principle of least privilege · Patch management strategy · Access control mechanisms · Common access control models

[↑ Back to top](#tdt4237-software-security)

## Web application security

A deep dive into common web vulnerabilities and how to prevent them.

### Web Security – Part 1

**Quiz:** [Web Security – Part 1](https://dev-quizmachine.itautomasjon.no/Quiz/Take/websecpart1) · [FlexiQuiz version](https://www.flexiquiz.com/SC/N/WebSecPart1)

**Topics:** Session hijacking techniques · Man-in-the-Middle (MITM) attack · Cross-Site Request Forgery (CSRF) · Cross-Site Scripting (XSS) · XSS protection for session hijacking · CSRF protection for session hijacking · CORS overview · CORS misconfiguration vulnerabilities · Server injection attack types · SQL injection defense via parameterization

### Web Security – Part 2

**Quiz:** [Web Security – Part 2](https://dev-quizmachine.itautomasjon.no/Quiz/Take/websecpart2) · [FlexiQuiz version](https://www.flexiquiz.com/SC/N/WebSecPart2)

**Topics:** File upload attacks · XSS mitigation techniques · Real-world CSRF example (Twitter) · CSRF mitigation strategies · Session cookie protection methods · Web server information leakage prevention · Risks of not using HTTPS · Clickjacking prevention · Email fraud prevention · Cookie protection rationale

### Web Security – Part 3

**Quiz:** [Web Security – Part 3](https://dev-quizmachine.itautomasjon.no/Quiz/Take/websecpart3)

**Topics:** HTTP vs cookie-based authentication · XSS, CSRF, and XSSI differences · Stored XSS vs Reflected XSS · CSRF and Referer header limitations · Action tokens in CSRF protection · Token and cookie combination defense · XSS prevention methods · HTTP header vulnerability rationale · HTTP header injection examples · Content-Type sniffing and XSS risks · Reducing XSS impact · Recommended XSS mitigation practices

### Web Security – Part 4

**Quiz:** [Web Security – Part 4](https://dev-quizmachine.itautomasjon.no/Quiz/Take/websecpart4)

**Topics:** Web security best practices · STRIDE threat model · Environmental creep · Access control models · Bell-LaPadula principles · Bell-LaPadula rules · SAML SSO components · SAML use cases · Stack overflow causes · Call stack behavior · Memory overflow types · Memory safety across languages · Unsafe defaults in C/C++ · Safe defaults in C# · Website copier tools · HTTrack and VisualWget usage · Web debugging proxies · Firefox Dev Tools and Fiddler · Security toolkits · Burp Suite, OWASP ZAP, Kali Linux · Google Dorking operators · SSRF attack scenarios · Rainbow table protection · Security by Design – goal · Least privilege principle · Threat modeling importance

[↑ Back to top](#tdt4237-software-security)
