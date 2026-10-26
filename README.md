

### 1. Protocols: Full Forms & One-Line Uses

* **HTTP (HyperText Transfer Protocol):** Transmits unencrypted web page data between a web browser and a web server.
* **HTTPS (HyperText Transfer Protocol Secure):** Encrypts web traffic using SSL/TLS to protect sensitive data during transmission.
* **FTP (File Transfer Protocol):** Transfers files between a client and a remote server over a network.
* **SMTP (Simple Mail Transfer Protocol):** Sends and routes outgoing emails across IP networks.
* **DNS (Domain Name System):** Resolves human-readable domain names (like `google.com`) into computer-friendly IP addresses.

---

### 2. Difference Between IPv4 and IPv6

| Feature | IPv4 | IPv6 |
| --- | --- | --- |
| **Address Length** | 32-bit numeric address | 128-bit hexadecimal address |
| **Format** | 4 decimal octets separated by dots (e.g., `192.168.1.1`) | 8 hexadecimal groups separated by colons (e.g., `2001:0db8::1`) |
| **Address Space** | $\approx 4.3 \times 10^9$ ($\approx 4.3$ billion addresses) | $\approx 3.4 \times 10^{38}$ (virtually inexhaustible) |
| **Configuration** | Configured manually or via DHCP | Supports stateless address autoconfiguration (SLAAC) and DHCPv6 |

---

### 3. `nslookup google.com` Output & Demonstration

Run the command in your terminal/command prompt:

```bash
nslookup google.com

```

**Typical Output:**

```text
Server:  dns.google
Address:  8.8.8.8

Non-authoritative answer:
Name:    google.com
Addresses:  2404:6800:4002:80b::200e
          142.250.193.142

```

* **Explanation:** The DNS resolver contacts name servers to resolve the domain name `google.com` into its IPv4 address (e.g., `142.250.193.142`) and its IPv6 address (e.g., `2404:6800:4002:80b::200e`).

---

### 4. HTTP Status Codes Explained

* **`200 OK`:** The request succeeded (e.g., the webpage loaded normally).
* **`301 Moved Permanently`:** The requested URL has permanently moved to a new location.
* **`400 Bad Request`:** The server could not understand the request due to invalid syntax.
* **`403 Forbidden`:** The server understands the request, but refuses to authorize access.
* **`404 Not Found`:** The requested resource does not exist on the server.
* **`500 Internal Server Error`:** The server encountered an unexpected condition that prevented it from fulfilling the request.

---

### 5. URL Anatomy Breakdown

Example URL: `[https://mail.google.com/mail/u/0/#inbox](https://mail.google.com/mail/u/0/#inbox)`

* **Scheme / Protocol (`https://`):** Specifies the protocol used to access the resource securely.
* **Subdomain (`mail.`):** A subdivision under the main domain dedicated to a specific service.
* **Second-Level Domain (`google`):** The primary brand or organization name.
* **Top-Level Domain / TLD (`.com`):** The domain category or extension.
* **Root / Apex Domain (`google.com`):** The combined TLD and primary domain.
* **Path (`/mail/u/0/`):** The exact path to the directory or file on the server.
* **Anchor / Fragment (`#inbox`):** An internal page reference/bookmark handled client-side.

