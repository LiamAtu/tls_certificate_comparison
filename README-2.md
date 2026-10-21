# 🔐 HTTPS Web Server: RSA vs ECC Certificates

![AWS](https://img.shields.io/badge/AWS%20EC2-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![TLS](https://img.shields.io/badge/TLS-2E7D32?style=for-the-badge&logo=letsencrypt&logoColor=white)

A networking project from my course at **ATU Galway**.

I set up a website on an AWS server and made it secure (HTTPS) using two types of certificate, **RSA** and **ECC**. Then I used **Wireshark** to watch the traffic between my browser and the server.

**Result:** the ECC certificate was much smaller than the RSA one (1,044 bytes vs 1,667 bytes).

---

## ECC Certificate

**The website working over HTTPS**
![ECC browser certificate](screenshots/ecc-01-browser-certificate.png)

**DNS lookup**
![DNS lookup](screenshots/ecc-02-dns-lookup.png)

**Client Hello**
![Client Hello](screenshots/ecc-03-client-hello-sni.png)

**Server certificate**
![Server certificate](screenshots/ecc-04-server-certificate-ecdsa.png)

**Session ticket**
![Session ticket](screenshots/ecc-05-session-ticket.png)

**TLS 1.3 connection**
![TLS 1.3](screenshots/ecc-06-tls13-hybrid-key-share.png)

---

## RSA Certificate

**The website working over HTTPS**
![RSA browser certificate](screenshots/rsa-01-browser-certificate.jpg)

**DNS lookup**
![DNS lookup](screenshots/rsa-02-dns-lookup.jpg)

**TLS handshake**
![Handshake](screenshots/rsa-03-handshake-overview.jpg)

**Server certificate**
![Server certificate](screenshots/rsa-04-server-certificate.jpg)

**TLS 1.3 connection**
![TLS 1.3](screenshots/rsa-05-tls13-client-hello.jpg)

---

## 🛠️ Tools
AWS EC2 · DNS · ZeroSSL · Wireshark

### 🤝 Connect With Me
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/liam-kapelianis-a42b3b403)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LiamAtu)
