# Cyber Security Internship — Task 1

## Objective
To scan the local network for open ports and understand potential security exposure.

## Tools Used
- Nmap v7.98
- Windows PowerShell

## Commands Executed
nmap -sS 192.168.1.0/24
nmap -sS 192.168.1.0/24 -oN scan-results.txt

## Results Summary

| IP Address | Open Ports | Services        | Device Type          |
|-------------|-------------|-----------------|-----------------------|
| 192.168.1.1 | 53, 443, 3517 | DNS, HTTPS, IAPP | Router (Zyxel) |
| 192.168.1.3 | None | — | Unknown device |
| 192.168.1.4 | 62078 | iPhone‑Sync | Apple mobile |
| 192.168.1.6 | 135, 139, 445 | MSRPC, NetBIOS, SMB | Local PC |

## Security Insights
- Router ports 53 & 443 are standard but should remain password‑protected.
- Windows SMB services should be disabled if not needed.
- No unauthorized open ports detected.

## Outcome
Learned to:
- Identify IPs and open ports on the local network.
- Understand service exposure.
- Perform basic risk analysis.
