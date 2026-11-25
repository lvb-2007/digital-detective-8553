## Mission 7-How computers communicate

## 1. Task / objective
Explain network types and concepts, observe connectivity and DNS, and describe
what happens when a browser opens a website.

## 2. Work completed

### Task 7.1 — Network concepts

| Concept | Explanation | Example |
|---|---|---|
| LAN | A network covering a small area | A home or school network |
| MAN | A network connecting sites across a city | A city-wide institutional network |
| WAN | A network spanning large geographic areas | The Internet |
| DNS | Resolves human-readable domain names to IP addresses | Looking up `example.com` |
| Router | Forwards traffic between networks | A home router connecting devices to an ISP |
| Protocol | Agreed rules for communicating | HTTPS for web traffic |
| Packet switching | Sends data as packets that can travel independently | Web data crossing multiple network links |
| Client-server | A client requests a service and a server responds | A browser requesting a webpage |

### Task 7.2 — Connectivity and DNS
I ran `ping -c 4 example.com`; all four packets received replies (0% packet
loss). `nslookup example.com` returned DNS records. The test domain's
addresses are omitted from this README because they are not needed to explain
the result.

### Task 7.3 — Opening a website
The browser checks whether it already has a usable DNS result. If not, it asks
a DNS resolver for the server address, connects to the server, negotiates
HTTPS when appropriate, sends an HTTP request, and receives the response.
The browser then interprets the returned HTML, CSS and scripts to display the
page.

## 3. Commands / tools used
- `ping -c 4 example.com` — checked connectivity; four replies and no packet
  loss were observed.
- `nslookup example.com` — observed DNS resolution.
- Terminal and VS Code — ran the commands and documented the results.
- Git — tracked and published mission work.

## 4. My understanding
LAN, MAN and WAN describe networks of increasing geographic scope. DNS maps
domain names to addresses, routers forward traffic, and protocols define how
devices communicate. Packet switching carries data in smaller units, while
the client-server model describes how a browser requests content from a
server. DNS lookup, connection setup, an HTTP request and the server response
work together to load a website.

## 5. Difficulties faced
It was difficult to distinguish network size categories and to put the
website-loading steps in the correct order.

## 6. How I resolved them
I compared each network type by its geographic coverage and broke website
loading into DNS lookup, connection, request and response steps.

## 7. Evidence / files
- This README contains the concept table and sanitized observations.


## 8. Commit details
- Correction commit: ` complete networking mission notes`