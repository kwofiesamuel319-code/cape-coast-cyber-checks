# Cape Coast Cyber Checks
13-day cyber security lab built 100% on Android phone using Termux

**Location:** Cape Coast, Ghana
**Tools:** Termux, Nmap, OpenSSL, ss
**Network:** MTN 4G LTE (Carrier NAT)

### Day 1-6: Setup
- Installed Termux, nmap, openssl
- Learned Linux basics on Android without root

### Day 7-12: Live Scans
- Target: scanme.nmap.org - Found 5 open ports (22,80,9929,31337, etc)
- Target: 127.0.0.1 (my phone) - 1000 ports closed - secure
- Target: 192.168.1.1 - 0 hosts on 4G (learned carrier NAT blocks LAN scans)

### Day 13: Hardening
- WhatsApp 2FA enabled
- Strong passwords with openssl rand
- GitHub portfolio created

### What I learned
Android 13 blocks /proc/net/tcp and ifconfig without root. Workaround: use `ss -t -a` and `nmap -sT 127.0.0.1`

---
Built by Kwofie Samuel | Cape Coast | Self-taught | September 2025