# Project Aikido

An integrated cybersecurity research platform focused on offensive security and AI red-teaming.

---

## Overview

Project Aikido combines hands-on hardware research, adversarial machine learning, and live threat intelligence infrastructure into a unified research environment. Each component is designed to inform the others — findings from physical hardware analysis feed into ML attack research, honeypot telemetry feeds into automated threat briefing, and all of it is documented and version-controlled as a living research record.

The name reflects the philosophy: like the martial art, the goal is to understand how attacks work at a fundamental level and use that knowledge defensively.

---

## Research Areas

### Hardware & Firmware Analysis
Physical teardown and low-level analysis of IoT and edge devices. Current target: TP-Link TC-7610 DOCSIS 3.0 cable modem (Broadcom SoC, MIPS architecture). Objectives include SPI Flash firmware extraction, binwalk analysis, and MIPS assembly reversing.

### Adversarial Machine Learning
Implementation and benchmarking of classic adversarial ML attacks against image classifiers and other models, followed by defense implementation and evaluation. Attack suite includes FGSM, PGD, Carlini-Wagner, and DeepFool.

### AI-Native Honeypot & Threat Intelligence
Live honeypot network with an AI analysis layer for automated TTP extraction, malware triage, and threat briefing generation. Includes a novel fake AI API endpoint designed to capture LLM-based exploitation attempts.

### Edge AI Red-Teaming
Attacking AI models running on physical edge hardware. Focus areas include model extraction, adversarial physical inputs, and side-channel analysis on devices running local inference stacks.

---

## Scope & Ethics

This project operates strictly within the following boundaries:

- All research is conducted on owned hardware and intentionally vulnerable environments
- No outbound attack traffic against systems I do not own or have explicit permission to test
- Responsible disclosure for any vulnerabilities discovered
- Ethical handling of any third-party data captured by research infrastructure

---

## Status

Active. Early stage. Hardware lab and infrastructure are being built out in parallel with foundational study in machine learning, assembly, and network security.

---

## Contact

GitHub: [codyAllanSec](https://github.com/codyAllanSec)
