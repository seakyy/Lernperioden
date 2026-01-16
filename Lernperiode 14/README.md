# [SiteShield](https://github.com/seakyy/siteshield)

In the next few LA's I will try to create a functional FLow between a Client app, a Server and a Website which will be hosted on a Raspberry Pi 5 with a Database. The goal of the project SiteShield is to develop an [EDR](https://www.microsoft.com/en-us/security/business/security-101/what-is-edr-endpoint-detection-response) 

## Languages used:
- C++ in CLient App (Used to read Windows API)
- Java in Server Backend (Universal and used to host it on [RP5](https://www.raspberrypi.com/products/raspberry-pi-5/))
- Anglar & JS Frontend (Website which will be available under [sitehsield.koteski.ch](https://siteshield.koteski.ch)

# Week 1 
In the first week my goal is to create an Public Key Infrastructure.
- [ ] Infrastructure: Create Public Key Infrastructure. Using OpenSSL to create a Root-CA. Generating a Server certificate for my Java Backend and a Client certificate for my C++ Agent.
- [ ] Backend: Set up a Java Spring Boot project. Configurate Tomcat for HTTPS with Client-Auth. Import of certificates in JKS or PKCS12 keystore.
- [ ] C++ Agent: Import HTTP CLient (either cpr or libcur1, idk which one yet) which sends a client certificate and a private key with every request. Goal here: successful handshake with the server.
- [ ] Backend: Database Design (PostgreSQL) for Devices and SecurityLogs. Create a Endpoint ```POST  /api/telematry```, which accepts xml/json.
- [ ] Security: Add validation in Backend. Check wether the "Common Name" in the certificate of the client device matches the registered CLient-ID (Hardware ID). This should prevent stealing of certificates.

