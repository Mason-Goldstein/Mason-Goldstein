# Mason Goldstein

**Cybersecurity Student | Linux & Network Security | Home Lab Builder**
Richmond, VA · Seeking cybersecurity and IT internship opportunities

---

### About

I am a Cybersecurity student at Randolph-Macon College focused on defensive security. I run a Raspberry Pi 5 home lab where I practice securing Linux systems, controlling network access, and self-hosting services, and I am building a personal AI assistant that integrates with it. My goal is to contribute to a security or IT operations team while continuing to grow my technical skills.

### Education

**Randolph-Macon College**, Ashland, VA
- Major: Cybersecurity
- Second Major: Religious Studies
- Minor: Computer Science

---

### Projects

#### ATLAS — Autonomous Tactical Learning and Assistance System *(in development)*
A voice-driven personal AI assistant with a cybersecurity focus that runs on Windows and manages my Raspberry Pi home lab.

```
Windows PC → ATLAS → SSH (Paramiko) → Tailscale → Raspberry Pi 5 → Docker containers
```

- **Model routing:** orchestrator that routes requests between local models and the Claude API, with a local-only mode to avoid API costs
- **Voice pipeline:** wake word detection (openWakeWord), speech-to-text (faster-whisper), and text-to-speech (Piper)
- **HUD dashboard:** native desktop app built with pywebview showing live system status
- **Home lab integration:** MQTT heartbeat metrics from the Pi and a remote-management layer over SSH that is read-only by default
- **Safety model:** read-only actions run automatically, changes require confirmation, and destructive actions require explicit approval
- **Next:** voice-triggered lab actions, tiered local models, and Pi-hole / DNS health monitoring

**Tools:** Python, Paramiko, MQTT, Tailscale, local LLMs, Claude API, pywebview

#### Raspberry Pi 5 Security Home Lab
A headless Ubuntu LTS lab I built and maintain for practicing Linux administration, networking, monitoring, and security.

- **Hardening:** SSH moved to a non-default port with key-based authentication only, UFW default-deny firewall, and Fail2Ban brute-force protection
- **Remote access:** private access through Tailscale with no services exposed to the public internet
- **Self-hosted services (Docker):**
  - Pi-hole for network-wide DNS filtering
  - Uptime Kuma for service monitoring
  - Portainer for container management
  - Homepage as a lab dashboard
  - OWASP Juice Shop for web application penetration testing practice

**Tools:** Ubuntu LTS, Docker, OpenSSH, UFW, Fail2Ban, Tailscale, Pi-hole

#### SkiOps — Maintenance Tracker Web App *(in development)*
A self-hosted web app for tracking maintenance on three personal watercraft. It is hosted on the home lab and reachable from phone or desktop through Tailscale.

- Interactive engine-bay diagram with editable markers for logging work by component
- Light, dark, and system themes

**Tools:** Python, Flask, SQLite, Docker Compose

---

### Coursework Projects

- **Networked Battleship (Python):** two-player client/server game with session IDs, ship placement, turn-based firing, server-side hit/miss results, and win/draw detection, implemented within an instructor-provided framework
- **Banking System (Python):** object-oriented `Client`, `BankAccount`, `CheckingAccount`, and `SavingsAccount` classes with input validation, account management, and interest calculation, extended across three projects with security as a main focus
- **Unit Testing (Python):** `unittest` test suites for transaction and banking logic

---

### Technical Skills

- **Operating Systems:** Linux (Ubuntu, command line, system administration), Windows
- **Security:** System hardening, firewall configuration, SSH security, intrusion prevention, DNS filtering, web application security practice
- **Networking:** Networking fundamentals, DNS, VPN / remote access, client/server programming
- **Infrastructure:** Docker, Docker Compose, self-hosting, service monitoring
- **Programming:** Python (Flask, unittest, Paramiko), C++ (coursework), SQL (SQLite)
- **Tools:** Git, GitHub, Tailscale, Pi-hole, Portainer, Uptime Kuma

### Continued Learning

- Hands-on security training through TryHackMe
- Ongoing study of network architecture and Linux hardening

### Contact

Open to internship and entry-level opportunities in cybersecurity and IT.
