# Nmap Cheatsheet

## Basic Scan Types
- TCP SYN Scan: `nmap -sS <target>`
- TCP Connect Scan: `nmap -sT <target>`
- UDP Scan: `nmap -sU <target>`
- TCP SYN Stealth Scan with OS detection: `nmap -sS -O <target>`
- TCP SYN Scan with version detection: `nmap -sV <target>`

## Service and Version Detection
- Version Detection: `nmap -sV <target>`
- Operating System Detection: `nmap -O <target>`
- Aggressive Scan (enables OS detection, version detection, script scanning, and traceroute): `nmap -A <target>`

## Output Options
- Normal output: `nmap <target>`
- Verbose output: `nmap -v <target>`
- Very verbose output: `nmap -vv <target>`
- Save output to file: `nmap -oN output.txt <target>`

## Host Discovery
- Ping Scan: `nmap -sn <target>`
- Ping Scan with TCP ACK packet: `nmap -PA <target>`
- ARP Scan (local network): `nmap -PR <target>`

## Timing Options
- Paranoid timing: `nmap -T0 <target>`
- Sneaky timing: `nmap -T1 <target>`
- Polite timing: `nmap -T2 <target>`
- Aggressive timing: `nmap -T4 <target>`
- Insane timing: `nmap -T5 <target>`

## Scripting Engine
- Run default scripts: `nmap -sC <target>`
- Run specific script: `nmap --script=<script-name> <target>`
- List available scripts: `ls /usr/share/nmap/scripts/`

## Port Specification
- Scan specific ports: `nmap -p <ports> <target>`
- Scan ports by protocol: `nmap -p <protocol>:<ports> <target>`

## Firewall Evasion
- Fragment packets: `nmap -f <target>`
- Randomize packet order: `nmap --randomize-hosts <target>`
- Use decoy addresses: `nmap -D RND:<number> <target>`

## Other Useful Options
- Disable DNS resolution: `nmap -n <target>`
- Show all packets sent and received: `nmap --packet-trace <target>`
- Enable OS detection without scanning ports: `nmap -O --osscan-limit <target>`

