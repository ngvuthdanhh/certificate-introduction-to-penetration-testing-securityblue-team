# Lab 02 — Scanning & Enumeration

## Objective
Discover live hosts, open ports and services; enumerate detailed information for attack planning.

## Prerequisites
- Lab VM or legally scoped target
- Nmap installed (or use an online lab)
- Basic shell familiarity

## Tools
- Nmap (primary)
- Masscan (optional, for large ranges)
- Nmap NSE scripts
- enum4linux, smbclient (for SMB)
- Nikto (web server enumeration)
- curl / httpie (basic HTTP checks)

## Steps
1. **Ping / host discovery:** run simple host discovery to identify live hosts.
   - `nmap -sn <target-range>` (lab-only)
2. **Port scan:** run a service/version detection scan.
   - `nmap -sC -sV -p- -oA scans/full <target>`  
   - Explain flags: `-sC` (default scripts), `-sV` (version), `-p-` (all ports)
3. **Target-specific scans:** run focused scans on discovered ports (web, SMB, SSH).
   - Web: `nmap --script=http-enum -p80,443 <target>`
4. **Banner grabbing & enumeration:** use NSE scripts and tools:
   - SMB: `enum4linux -a <target>`
   - HTTP: Nikto, `curl -I`, directory brute with `gobuster` (lab target only)
5. **Document:** record open ports, versions, and potential vulnerable services.

## Deliverables
- Nmap output files (or summarized results)
- Enumeration checklist (services, versions, likely misconfigurations)
- Short prioritization (which service to target first and why)

## Safety & Legal
- Limit aggressive scans to lab environments. Masscan and full-port scans on public targets may be disruptive.
