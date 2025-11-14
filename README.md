How It Works:
User enters a message and selects a protocol (HTTPS, HTTP, FTP, SSH...).
The simulator encapsulates the packet layer by layer, generating:
Application: method, status code, content type, user agent
Presentation: TLS handshake, encryption, cipher suite
Session: session ID, tokens, timeout settings
Transport: ports, TCP flags, sequence numbers
Network: IP addressing, TTL, routing
Data Link: MAC, FCS, VLAN
Physical: medium, bitrate, encoding
The packet is transmitted and analyzed with deep packet inspection.
Threats such as MitM, abnormal TTL, SYN-FIN patterns, SSH brute-force behavior are automatically flagged.
The packet is then decapsulated back up the OSI layers.

How to run:
Just open index.html in any modern browser (Chrome, Safari, Edge, Firefox). No server required.