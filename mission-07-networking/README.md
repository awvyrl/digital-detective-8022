# Mission 7 - Computer Networks

## 1. Task / objective
Explain core computer networking concepts and network types, perform privacy-safe connectivity and DNS lookup tests in Terminal, and trace the step-by-step communication process when opening a website.

## 2. Work completed
* Completed a reference table defining LAN, MAN, WAN, DNS, router, protocol, packet switching, and the client-server model with examples.
* Ran `ping` and `nslookup` against `example.com` in Terminal and documented what each tool reveals without exposing private network information.
* Wrote a 6-step walkthrough explaining how a browser loads a webpage using client, server, DNS, router, and protocol concepts.

## 3. Commands / tools used
* `ping -c 4 example.com` — Sends 4 test packets to `example.com` to check reachability, round-trip latency, and packet loss.
* `nslookup example.com` — Queries DNS to resolve the domain name `example.com` into its numerical IP addresses.
* **Git (`git add`, `git commit`, `git push`)** — Stages, commits, and pushes Mission 7 documentation to GitHub.

## 4. My understanding

### Task 7.1 - Explain Network Concepts

| Concept | Explain it in your own words | Example |
| :--- | :--- | :--- |
| **LAN** | A Local Area Network covering a small physical space such as a home, classroom, or hostel floor. | Devices connected to the same local Wi-Fi router. |
| **MAN** | A Metropolitan Area Network spanning a city or a large multi-building campus. | A fiber network linking multiple university buildings across a city. |
| **WAN** | A Wide Area Network connecting devices and smaller networks across vast geographical distances. | The global Internet. |
| **DNS** | The Domain Name System, which translates human-readable website names into numerical IP addresses. | Translating `example.com` into its server IP address. |
| **Router** | A networking device that connects separate networks and forwards data packets toward their destination. | A home/hostel Wi-Fi router connecting a LAN to an ISP's WAN. |
| **Protocol** | A standardized set of rules defining how devices format, transmit, and receive data. | HTTPS, TCP/IP, or DNS. |
| **Packet switching** | Breaking large data into small chunks (packets) that travel independently across networks and reassemble at the destination. | Loading a webpage or streaming video over the internet. |
| **Client-server** | A communication model where a client device requests a service or file and a remote server processes and returns it. | A web browser (client) requesting a repository page from GitHub (server). |

---

### Task 7.2 - Observe Network Information
* **What a connectivity test (`ping -c 4 example.com`) helps you check:** It verifies whether my computer can successfully reach a remote host over the internet, measures the round-trip response time (latency) in milliseconds, and confirms that 0% of packets were lost.
* **What information a DNS lookup (`nslookup example.com`) displays:** It shows the DNS resolver answering the query along with the public IPv4 and IPv6 addresses mapped to `example.com`.
* **Role of DNS when entering a website name in a browser:** Computers route traffic using numerical IP addresses rather than English domain names. When I type a website URL, DNS acts like an internet directory that looks up and returns the server's IP address so my browser knows where to connect.

---

### Task 7.3 - What Happens When You Open a Website?
1. **User Request (Client):** I type a URL (such as `https://example.com`) into my web browser, which acts as the **client**.
2. **Domain Name Lookup (DNS):** Because my browser needs a numerical IP address to locate the website, it queries a **DNS** server to translate `example.com` into the destination server's IP address.
3. **Local Routing:** My computer packages the request and sends it through my local network to my **router**, which forwards the traffic onto my internet service provider's network.
4. **Network Transport via Protocols:** Following standard internet **protocols** (such as TCP/IP and HTTPS), the request travels as small data packets across multiple routers to reach the target web **server**.
5. **Server Processing & Response:** The web **server** receives the HTTPS request, locates the requested webpage files (HTML, CSS, images), and sends them back in packets toward my computer's connection.
6. **Rendering the Page:** My browser (the **client**) receives the response packets, reassembles the files, and renders the visual webpage on my screen.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
* `mission-07-networking/README.md`

## 8. Commit details
Committed with message: `"Explain networking concepts and website communication"` and pushed to GitHub.