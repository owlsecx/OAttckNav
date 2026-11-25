# 🦉 OAttckNav

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Security-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OAttckNav** — part of the OwlSec Toolkit.

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OAttckNav puts the MITRE ATT&CK Enterprise dataset (706 techniques, 174 groups) in your terminal. You can look up techniques and threat groups, build official ATT&CK Navigator layers, and grade your detection coverage. It compares your coverage with a specific group's TTPs to show the gaps you need to close.

---

## ✨ Features

- Technique and threat-group search and lookup across the full Enterprise dataset
- Builds ATT&CK Navigator v4.5 layer JSON from a group, platform, technique-ID list or keyword
- Coverage scoring per tactic with a grade and gap findings
- Coverage vs. threat-group comparison showing the uncovered techniques that group uses
- Layer merge and diff, plus technique prevalence across all groups ("top TTPs")
- ASCII tactic matrix / heatmap and reports in TXT / JSON / Markdown / CSV

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OAttckNav                                  # interactive menu
./OAttckNav --technique T1059
./OAttckNav --group APT29 --layer apt29.json
./OAttckNav --coverage my_layer.json --vs APT29
./OAttckNav --prevalence
```

Run `./OAttckNav --help` for the full list of options.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*

---

## 🔍 Verification & Transparency

This tool is closed-source. These files let you see exactly what is inside it,
without the source:

- [`SBOM.cdx.json`](SBOM.cdx.json) — CycloneDX inventory: SHA-256 of this
  binary, the Go toolchain version it was built with, and every bundled
  component with its exact version and license. Feed it to Grype, Trivy or
  Dependency-Track to audit our dependencies for CVEs yourself.
- [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md) — the full license text
  of every third-party component, extracted from this binary.

Release signing, GPL compliance and vulnerability reporting:
[**TRUST.md**](https://github.com/owlsecx/owl-os/blob/main/TRUST.md)
