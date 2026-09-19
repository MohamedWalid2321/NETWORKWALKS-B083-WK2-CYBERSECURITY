# 🔎 Footprinting, Reconnaissance & Network Scanning

A practical cybersecurity reconnaissance project focused on **footprinting, information gathering, web enumeration, DNS reconnaissance, and network scanning** using multiple security tools.

This project was completed as part of the **NETWORKWALKS Cybersecurity Internship — Batch B083**.

---

## 📌 Overview

The project demonstrates a structured reconnaissance process using multiple tools to gather information about a target and analyze its externally accessible infrastructure.

The reconnaissance activities include:

* Domain footprinting
* DNS enumeration
* Web technology identification
* HTTP header inspection
* Web Application Firewall detection
* Host discovery
* Network scanning
* Network topology visualization

---

## 🧰 Tools Used

| Tool              | Purpose                                                      |
| ----------------- | ------------------------------------------------------------ |
| **WHOIS**         | Domain registration and information gathering                |
| **Nslookup**      | DNS queries and domain resolution                            |
| **DNSRecon**      | DNS enumeration                                              |
| **WhatWeb**       | Web technology fingerprinting                                |
| **cURL**          | HTTP response and header inspection                          |
| **WAFW00F**       | Web Application Firewall detection                           |
| **Nmap / Zenmap** | Host discovery, network scanning, and topology visualization |

---

## 🔬 Reconnaissance Process

The project follows a practical reconnaissance workflow:

```text
                    Target
                       │
                       ▼
              ┌─────────────────┐
              │   Footprinting  │
              └────────┬────────┘
                       │
              ┌────────┴────────┐
              ▼                 ▼
           WHOIS            DNS Recon
                                │
                    ┌───────────┴───────────┐
                    ▼                       ▼
                Nslookup                DNSRecon
                    │                       │
                    └───────────┬───────────┘
                                ▼
                       Web Reconnaissance
                                │
                ┌───────────────┼───────────────┐
                ▼               ▼               ▼
             WhatWeb           cURL          WAFW00F
                │               │               │
                └───────────────┼───────────────┘
                                ▼
                       Network Scanning
                                │
                           Nmap / Zenmap
                                │
                                ▼
                       Network Topology
```

---

## 🌐 Domain & DNS Reconnaissance

### WHOIS

WHOIS was used to gather publicly available domain registration information.

```bash
whois <target>
```

### Nslookup

Nslookup was used to perform DNS queries and resolve domain-related information.

```bash
nslookup <target>
```

### DNSRecon

DNSRecon was used for DNS enumeration and reconnaissance.

```bash
dnsrecon -d <target>
```

---

## 🖥️ Web Reconnaissance

### WhatWeb

WhatWeb was used to identify technologies and components associated with the target website.

```bash
whatweb <target>
```

### cURL

HTTP response headers were inspected using:

```bash
curl -I <target>
```

This can provide information such as HTTP status codes, server information, cookies, redirects, and security-related headers.

### WAFW00F

WAFW00F was used to identify whether a Web Application Firewall was present.

```bash
wafw00f <target>
```

---

## 📡 Network Scanning

### Nmap / Zenmap

Nmap was used for network discovery and scanning, while Zenmap provided a graphical interface for working with Nmap and visualizing the discovered network.

The scanning process included:

* Host discovery
* Port scanning
* Service identification
* Network mapping
* Topology visualization

Example:

```bash
nmap <target>
```

---

## 📂 Repository Structure

```text
.
├── screenshots/
│   ├── curl_results.PNG
│   ├── dnsrecon_results.PNG
│   ├── nslookup_results.PNG
│   ├── ping_scan.PNG
│   ├── topology.PNG
│   ├── wafw00f_results.PNG
│   ├── whatweb_results.PNG
│   └── whois_results.PNG
│
├── <report>
│
└── README.md
```

The `screenshots/` directory contains the results and evidence collected during the reconnaissance and scanning activities.

---

## 📊 Reconnaissance Coverage

| Area                  | Tool               |
| --------------------- | ------------------ |
| Domain Footprinting   | WHOIS              |
| DNS Enumeration       | Nslookup, DNSRecon |
| Web Fingerprinting    | WhatWeb            |
| HTTP Header Analysis  | cURL               |
| WAF Detection         | WAFW00F            |
| Host Discovery        | Nmap               |
| Network Scanning      | Nmap / Zenmap      |
| Network Visualization | Zenmap             |

---

## 🎯 Learning Objectives

This project provided hands-on experience with:

* Performing structured reconnaissance
* Gathering information from publicly accessible services
* Enumerating DNS information
* Fingerprinting web technologies
* Analyzing HTTP response headers
* Identifying WAF technologies
* Discovering hosts and network services
* Visualizing network topology
* Documenting reconnaissance results

---

## ⚠️ Responsible Use

The techniques and tools demonstrated in this repository should only be used against systems and networks that you **own or have explicit authorization to assess**.

This project is intended for **cybersecurity education, authorized security assessments, and controlled laboratory environments**.

---

## 👤 Author

**Mohamed Walid**

Cybersecurity | Penetration Testing | Network Security

---

## 📚 Project Information

**Program:** NETWORKWALKS Cybersecurity Internship
**Batch:** B083
**Project:** Footprinting, Reconnaissance & Network Scanning
