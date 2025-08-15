+++
date = '2025-08-03T00:38:44-07:00'
title = "About"
menu = "main"
weight = 2
hideReply = true
author = "Smith Barlow"
description = "Smith Barlow's About Page"
+++
# About Me

## Projects
__Homelab__\
*August 2025*
- Deployed and configured OPNsense as the main router and firewall, setting up VLANs, appropriate subnets, DHCP, and firewall rules to segment and secure homelab traffic.
- Utilized Proxmox to host virtual machines for labs and services, learning virtualization, resource allocation, and snapshot management—accomplished utilizing LXC containers and KVM virtual machines.
- Created a SOC lab environment using Kali Linux for vulnerability assessment, a Windows target for exploitation, and the Wazuh stack for real-time detection and prevention.
- Configured OPNsense firewalling with strict baselines—ensure intervlan traffic is strict and within scope.
- Utilized Wireguard to secure sensitive traffic from self-hosted services to VPS proxy—terminated with TLS 1.2/1.3 certificates.

__VPS__\
*August 2025*
- Deployed a strict firewall policy: default-deny incoming, a strict UFW ruleset only allowing essential ports (non-standard IP-bound SSH port), with Tor service bound to localhost and isolated from public interfaces.
- Obtained an [A+ SSL Labs Score](https://www.ssllabs.com/ssltest/analyze.html?d=smithbarlow.xyz), configured Let's Encrypt TLS (TLS 1.2/1.3) with strong AEAD ciphers, implemented HSTS preload, instituted DNSSEC to prevent MITM attacks, and restrictive CAA policies to prevent rogue issuance.
- Secured Nginx with tight content security policies, method restrictions (GET/HEAD only), rate-limiting, appropriate header limits, and privacy-respecting security headers.
- Deployed kernel-level security via extensive sysctl settings, unused protocol and module blacklisting (modprobe blocklist), and AppArmor confinement for Nginx and Tor to limit post-exploit impact.
- Incorporated a strong chain of trust: a signed Tor mirror statement, mirrored public GPG keys, and SHA-512 checksum proofs—all implemented across DNS TXT records and a [GitHub mirror](https://github.com/smithbarlow/smithbarlow.gpg).

### Verification

```
dig smithbarlow.xyz ANY +noall +answer +authority +additional +dnssec
curl -vkI https://smithbarlow.xyz
```

## Events
__Summer Cyber Tech Track__\
__*Ken Garff Esports*__\
*July 2025*
-  Participated in the CyberPatriot Windows and Linux security competitions, identifying and fixing security vulnerabilities.
- Learned Linux fundamentals such as command-line navigation, file system structure, and user permissions—including SSH hardening, network hardening (ufw), and managing malicious system services (systemctl).
- Gained practical experience with Linux and Windows security concepts, such as: account management, patching, service auditing, basic firewall deployment, and intrusion prevention methodologies.

## Certifications
- [CyberPatriot (AFA) - Standard AFA CyberCamp ](https://smithbarlow.xyz/CyberPatriot-Certificate-Smith-Barlow.pdf)

## Education
> __High School Diploma - Northridge High School__\
> August, 2025 - May, 2028
