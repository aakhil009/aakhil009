- 👋 Hi, I’m @aakhil009
Generate OpenSSL
  - openssl genpkey -algorithm RSA -out private_key.pem -aes256     --> Generate private key 
  - openssl req -new -key private_key.pem -out csr.pem              --> Generate CSR (Certificate Signing Request)
  - openssl x509 -req -days 365 -in csr.pem -signkey private_key.pem -out certificate.crt           --> Generate Self-Signed Certificate (X.509)
  - openssl rsa -in private_key.pem -outform PEM -out private_key.crt                               --> Export Private Key and Certificate to Separate CRT Files
  - 
 
