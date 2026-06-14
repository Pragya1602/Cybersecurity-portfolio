# Cybersecurity Portfolio

A collection of hands-on projects focusing on systems security, network protocols, and vulnerability analysis.

## Projects

### 1. Keystroke Telemetry Monitor (OS API Hooks)
A low-level system utility designed to capture and log asynchronous hardware input events. This project explores how operating systems handle input processing queues and file I/O operations.

* **Language:** Python
* **Core Concepts:** Windows API hooking (`SetWindowsHookEx`) / Linux input event sub-system (`/dev/input/`), multi-threading, and local text-stream logging.
* **Security Context:** Demonstrates the mechanics of spyware execution to better understand host-based detection engineering and Endpoint Detection and Response (EDR) telemetry bypasses.

---

### 2. OverTheWire: Natas Web Exploitation
Overview
A series of hands-on security engineering lads focused on identifying, exploiting, and remediating server-side web vulnerabilities. It covers backend execution logic (PHP), database interactions, and network state management via manual code audits and custom automation scripts.

Core Features
Session Tampering: Reverses and modifies client-side cookies, tracking tokens, and HTTP headers to bypass authentication gates.
Source Code Auditing: Reviews raw PHP backends to detect logic flaws, un-sanitized inputs, and weak custom cryptographic implementations.
Information Disclosure: Exploits server misconfigurations, including open Directory Indexing and exposed robots.txt paths.
Exploit Automation: Develops modular Python scripts using the requests library for automated payload delivery and data extraction.
