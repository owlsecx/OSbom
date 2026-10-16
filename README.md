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

Software Bill of Materials generator & offline dependency advisory matcher

---

## ✨ Features

- Lockfile parsers — requirements*.txt, Pipfile.lock, poetry.lock, package-lock.json / npm-shrinkwrap, yarn.lock (v1 + berry), pnpm-lock.yaml (basic), go.mod / go.sum, Cargo.lock, Gemfile.lock, composer.lock — name, version, scope, ecosystem
- Recursive project discovery with exclude list, depth limit and per-file error isolation
- Package URL (purl) generation per ecosystem
- SBOM export — CycloneDX 1.5 JSON, SPDX 2.3 JSON, CSV inventory, Markdown table, native OSbom JSON
- License hints — LICENSE/COPYING classifier for common SPDX ids + lockfile license metadata
- Offline advisory DB — built-in demo rows plus external JSON (--advisories), simple OSV-lite import, optional --fetch-advisories URL (explicit, timeout)
- Version-range matcher (=, ==, <, <=, >, >=, !=, comma AND, || OR, wildcard *) across ecosystems
- SHA-256 hash inventory of lockfiles and artifacts
- SBOM diff — added / removed / updated packages
- Policy gate — --fail-on severity, allowlist, ignored advisory ids, exit codes for CI
- Save chooser (~/OSbom) + clipboard summary

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OSbom
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
