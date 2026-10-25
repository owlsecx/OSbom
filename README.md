# 🦉 OSbom

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OSbom** — Software Bill of Materials & Advisories

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OSbom is a software bill-of-materials generator and offline vulnerability matcher. It parses lockfiles across many ecosystems, generates CycloneDX and SPDX SBOMs, and matches packages against offline advisory data with a version-range engine. It supports SBOM diffing and policy gates for CI.

---

## ✨ Features

- Lockfile parsers for Python, npm/yarn/pnpm, Go, Cargo, Gemfile and Composer ecosystems
- Package URL (purl) generation and recursive project discovery
- SBOM export as CycloneDX 1.5, SPDX 2.3, CSV, Markdown and native JSON
- Offline advisory database with optional external feeds and a version-range matcher
- License hints and SHA-256 hash inventory of lockfiles and artifacts
- SBOM diff and a policy gate (fail-on severity, allowlist, ignore ids) for CI

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OSbom -p ./project -f cyclonedx -o sbom.json
./OSbom -p ./project --fail-on high
./OSbom --diff old-sbom.json new-sbom.json
./OSbom --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
