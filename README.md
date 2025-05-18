# ICExpose

Uses WebRTC to "decloak" a user's local and real public IP addresses (behind a VPN, proxy etc.) using ICE candidates via a STUN server.

* **STUN Server:** Sends WebRTC requests to a STUN server to discover public-facing IPs.                                
* **ICE Candidates:** Captures ICE candidates and extracts IP, port, protocol, and candidate type.
---

## Usage

* **Host the `icexpose.html file on a web server.**
* **Open the `icexpose.html file in a browser.**
* **Wait for WebRTC to gather ICE candidates.**
* **View the detected IPs and associated metadata in the table.**

### Example Output

| IP Address   | Port  | Protocol | Candidate Type |
| ------------ | ----- | -------- | -------------- |
| 192.168.1.10 | 53725 | udp      | host           |
| 203.0.113.5  | 19302 | udp      | srflx          |

---

## Notes

* This tool **does not send data to any third-party server.**
* All IP detection is performed locally within the browser.
