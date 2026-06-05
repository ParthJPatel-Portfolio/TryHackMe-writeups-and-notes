# HTTP in Detail TryHackMe Room

## What is HTTP?

HTTP (HyperText Transfer Protocol) is the protocol used for communication between web browsers and web servers. It defines how requests are sent from a client and how responses are returned from a server.

Common data transferred through HTTP includes:

- HTML pages
- Images
- Videos
- CSS files
- JavaScript files

HTTP operates on port 80 by default and does not encrypt data during transmission.

## What is HTTPS?

HTTPS (HyperText Transfer Protocol Secure) is the secure version of HTTP. It uses TLS/SSL encryption to protect data exchanged between clients and servers.

HTTPS provides:

- Confidentiality through encryption
- Integrity by preventing data modification
- Authentication through digital certificates

HTTPS operates on port 443 by default.

## HTTP vs HTTPS

| HTTP | HTTPS |
|--------|--------|
| Unencrypted | Encrypted |
| Port 80 | Port 443 |
| Less secure | More secure |
| No certificate validation | Uses SSL/TLS certificates |

## Key Takeaways
- HTTP is the foundation of web communication.
- HTTPS secures web traffic using encryption.
- Modern websites should use HTTPS to protect user data and verify website authenticity.
