# Lab 01 — Reconnaissance (OSINT & Passive Recon)

## Objective
Practice passive information gathering and OSINT techniques to build an initial target profile without interacting with the target directly.

## Prerequisites
- Internet access
- Browser + privacy mode
- Account on TryHackMe / lab VM (use a legal target)
- Note-taking tool for evidence (Markdown)

## Tools (suggested)
- Google dorking (search operators)
- OSINT Framework (web)
- whois, dig (local)
- Shodan / Censys (accounts recommended)
- theHarvester, recon-ng (optional)

## Steps
1. **Define scope & rules:** confirm target is your lab (Do NOT run against real targets).
2. **Passive search:** use Google dorks to find exposed info (e.g., site:, filetype:, intitle:).
3. **WHOIS & DNS:** run `whois` and `dig` to gather registrar and DNS records.
4. **Public footprint:** check social media, LinkedIn, GitHub for leaked info or credentials.
5. **Shodan/Censys:** search for public-facing services and banners (only on allowed IPs).
6. **Aggregate findings:** build a target profile (domains, subdomains, tech stack hints, public endpoints).
7. **Record evidence:** save screenshots, query outputs, and DFI (data flow/infrastructure notes).

## Deliverables
- Target profile document (Markdown) with:
  - Domain/subdomains found
  - Public services & banners
  - Potential entry points (from OSINT)
  - Screenshots and commands used
- Short risk assessment (low/medium/high) for each finding

## Safety & Legal
- Only perform recon on targets you own or explicit lab targets (TryHackMe boxes, local VMs).
- Maintain a log of every action and timestamp.
