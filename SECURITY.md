# Security notes

This repository is a client-side demonstration, not a production auction or payment system.

- Admin sign-in using embedded credentials has been disabled for this public copy. The original source contained a hardcoded admin email and password; those values have not been included here.
- User and seller accounts are stored in browser storage. Client-side password hashing or checks are not a substitute for server-side authentication.
- OTP and CAPTCHA flows are demonstrations only. No real SMS delivery or independent CAPTCHA validation is performed.
- Payment screens simulate checkout and must not be used to collect or process real payment details.
- Uploaded documents and auction records are handled in the browser and are not securely stored on a server.

Before production use, implement server-side authentication and authorization, secure file storage, a real OTP provider, a verified CAPTCHA service, and a payment gateway integration. Keep all secrets in server-side environment variables and never commit them to a public repository.
