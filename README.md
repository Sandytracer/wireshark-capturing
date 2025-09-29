# wireshark-capturing
Here’s a concise summary of your findings and packet details from **Task 5: Network Traffic Analysis with Wireshark**, Santhiya:

---

## 🧾 Summary of Findings

During the packet capture session, several key protocols were identified and analyzed. These protocols are fundamental to everyday internet communication and provide insight into how data travels across networks.

### 🔍 Protocols Observed

| Protocol | Function | Key Observations |
|---------|----------|------------------|
| **HTTP** | Web traffic (GET/POST requests) | Captured requests to websites like `example.com`, showing headers and response codes |
| **DNS** | Resolves domain names to IP addresses | Queries to resolve domains such as `google.com`, with responses containing IP addresses |
| **TCP** | Reliable data transmission | Included 3-way handshake (SYN, SYN-ACK, ACK) and data segments between client and server |
| **UDP** | Lightweight, connectionless transport | Used in DNS queries; faster but less reliable than TCP |
| **ICMP** | Diagnostic messages (e.g., ping) | Echo requests and replies used to test connectivity to external servers |

---

## 📦 Packet Details

Here are examples of packet-level insights:

- **HTTP Packet**
  - Source IP: `192.168.1.10`
  - Destination IP: `93.184.216.34`
  - Method: `GET /index.html`
  - Status: `200 OK`

- **DNS Query**
  - Query: `A google.com`
  - Response: `142.250.182.206`
  - Protocol: UDP
  - Port: 53

- **TCP Handshake**
  - SYN from client to server
  - SYN-ACK from server to client
  - ACK from client to server
  - Port: 443 (HTTPS)

- **ICMP Ping**
  - Type: Echo Request
  - Reply from: `8.8.8.8`
  - Round-trip time: ~30ms
