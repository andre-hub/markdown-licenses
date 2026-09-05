# Markdown Licenses

[🇩🇪 Deutsche Version](README.de.md)

A curated collection of open-source and open-content licenses formatted in clean, standard Markdown — ready to drop into any repository as `LICENSE.md`.

All files use standard ASCII quotes, UTF-8 encoding, and canonical [SPDX identifiers](https://spdx.org/licenses/) for reliable compatibility with automated tooling (REUSE, ScanCode, GitHub).

---

## License Categories & How to Choose

Understanding license families helps you pick the right terms for your project:

### 1. Permissive
* **Key traits:** Minimal restrictions; allows integration into proprietary software; only requires preserving copyright notices and disclaimers.
* **Top choices:**
  * **MIT:** The industry standard — simple, lightweight, maximum adoption.
  * **Apache 2.0:** Adds explicit patent grants and trademark protection; ideal for enterprise and multi-contributor projects.
  * **BSD 3-Clause / BSD 2-Clause:** Reliable BSD variants, with or without non-endorsement protections.
  * **Boost 1.0 / 0BSD:** Eliminate attribution requirements for compiled binary distributions.
  * **Blue Oak 1.0:** Plain-English, modern permissive terms.

### 2. Public Domain & Fallbacks
* **Key traits:** Dedicated to the public domain with no rights reserved, paired with an unconditional worldwide fallback license for jurisdictions that disallow rights waiving.
* **Top choices:**
  * **CC0 1.0:** Universal public domain dedication, standard for open data, models, and public-facing assets.
  * **The Unlicense:** Public domain dedication specifically tailored for software code.

### 3. File-Level & Library Copyleft (Weak Copyleft)
* **Key traits:** Modifications to the licensed files/library must remain open source under the same license, but your larger application or proprietary codebase remains unaffected.
* **Top choices:**
  * **MPL 2.0 (Mozilla Public License):** Clean file-boundary copyleft, very corporate-friendly.
  * **LGPL 3.0 / 2.1:** Standard for shared libraries; dynamic linking does not infect the proprietary host program.
  * **EPL 2.0:** Popular in the Java and enterprise tooling ecosystem with secondary license provisions.
  * **EUPL 1.2:** Tailored for European public administrations, legally equivalent across 23 official EU languages.

### 4. Strong Copyleft
* **Key traits:** Any derivative work or statically/dynamically bundled software must also be distributed under the same license. Guarantees that code stays free.
* **Top choices:**
  * **GPL 3.0:** Full protection against proprietary closing, includes express patent grants and anti-tivoization clauses.
  * **GPL 2.0:** Legacy standard (used notably by the Linux kernel); strictly requires source disclosure upon binary distribution.

### 5. Network / SaaS Copyleft
* **Key traits:** Closes the "SaaS / Application Service Provider loophole". Users interacting with the software over a network (e.g. web apps, cloud services) are entitled to receive the complete corresponding source code.
* **Top choices:**
  * **AGPL 3.0:** The premier choice for cloud backends, databases, and hosted web applications where software is run as a service rather than distributed as binaries.

### 6. Documentation, Media & Open Data
* **Key traits:** Tailored for creative materials, documentation, and database rights rather than executable binary code.
* **Top choices:**
  * **CC-BY 4.0:** Permissive for docs, tutorials, guides, and datasets (attribution required).
  * **CC-BY-SA 4.0:** Share-alike copyleft for documentation, wikis, and open publications.
  * **ODbL 1.0:** Specialized copyleft protecting structured database contents (e.g., OpenStreetMap).

---

## Quick Decision Guide

| Project Goal | Recommended License | Why? |
| :--- | :--- | :--- |
| **Maximum adoption & minimal friction** | [MIT](mit.md) | Most popular open-source license; effortless adoption in commercial software. |
| **Enterprise software with patent protection** | [Apache-2.0](apache-2.0.md) | Explicit grant of patent rights and trademark preservation. |
| **C/C++ library without binary attribution** | [Boost 1.0](boost-1.0.md) / [0BSD](0bsd.md) | No requirement to embed notices into compiled binary distributions. |
| **Unconditional public domain** | [CC0 1.0](cc0-1.0.md) / [The Unlicense](unlicense.md) | Waives all rights with a robust global fallback. |
| **Library / Framework (protect library, allow proprietary host)** | [MPL-2.0](mpl-2.0.md) or [LGPL-3.0](lgpl-3.0.md) | Improvements to the library stay open; larger application remains independent. |
| **European public sector** | [EUPL-1.2](eupl-1.2.md) | Tailored to EU legal framework with 23 legally binding language translations. |
| **Prevent proprietary enclosure (desktop/tools)** | [GPL-3.0](gpl-3.0.md) | Complete copyleft ensuring derivative works remain open source. |
| **Web services & cloud backends (SaaS protection)** | [AGPL-3.0](agpl-3.0.md) | Prevents running modified code as a cloud service without sharing source code. |
| **Documentation, guides & media** | [CC-BY-4.0](cc-by-4.0.md) / [CC-BY-SA-4.0](cc-by-sa-4.0.md) | Clear terms designed specifically for non-software creative assets. |
| **Open database & structured datasets** | [ODbL-1.0](odbl-1.0.md) | Protects dataset rights and database structures. |

---

## Quick Reference

| License | SPDX ID | File | Category / Description |
| :--- | :--- | :--- | :--- |
| **MIT** | `MIT` | [`mit.md`](mit.md) | Permissive, short, widely used |
| **Apache 2.0** | `Apache-2.0` | [`apache-2.0.md`](apache-2.0.md) | Permissive with explicit patent & trademark grant |
| **BSD 3-Clause** | `BSD-3-Clause` | [`bsd-3-clause.md`](bsd-3-clause.md) | Permissive with non-endorsement clause |
| **BSD 2-Clause** | `BSD-2-Clause` | [`bsd-2-clause.md`](bsd-2-clause.md) | Simplified permissive without endorsement clause |
| **0BSD** | `0BSD` | [`0bsd.md`](0bsd.md) | Zero-clause permissive, no attribution in binaries |
| **ISC** | `ISC` | [`isc.md`](isc.md) | Functionally equivalent to BSD 2-Clause / MIT |
| **Boost 1.0** | `BSL-1.0` | [`boost-1.0.md`](boost-1.0.md) | Permissive, exempts binaries from attribution |
| **Blue Oak 1.0** | `BlueOak-1.0.0` | [`blueoak-1.0.0.md`](blueoak-1.0.0.md) | Modern plain-language permissive |
| **CC0 1.0** | `CC0-1.0` | [`cc0-1.0.md`](cc0-1.0.md) | Public domain dedication & fallback |
| **The Unlicense** | `Unlicense` | [`unlicense.md`](unlicense.md) | Public domain dedication for software |
| **MPL 2.0** | `MPL-2.0` | [`mpl-2.0.md`](mpl-2.0.md) | Weak copyleft (file-level) |
| **LGPL 3.0** | `LGPL-3.0-or-later` | [`lgpl-3.0.md`](lgpl-3.0.md) | Weak copyleft (library linking permitted) |
| **LGPL 2.1** | `LGPL-2.1-or-later` | [`lgpl-2.1.md`](lgpl-2.1.md) | Legacy library copyleft (C/C++ libraries) |
| **EPL 2.0** | `EPL-2.0` | [`epl-2.0.md`](epl-2.0.md) | Weak copyleft with secondary license compatibility |
| **EUPL 1.2** | `EUPL-1.2` | [`eupl-1.2.md`](eupl-1.2.md) | European Union copyleft, 23 official languages |
| **GPL 3.0** | `GPL-3.0-or-later` | [`gpl-3.0.md`](gpl-3.0.md) | Strong copyleft with patent & anti-tivoization terms |
| **GPL 2.0** | `GPL-2.0-only` | [`gpl-2.0.md`](gpl-2.0.md) | Strong copyleft (Linux kernel standard) |
| **AGPL 3.0** | `AGPL-3.0-or-later` | [`agpl-3.0.md`](agpl-3.0.md) | Network copyleft for network/SaaS software |
| **CC-BY 4.0** | `CC-BY-4.0` | [`cc-by-4.0.md`](cc-by-4.0.md) | Permissive for documentation, data & media |
| **CC-BY-SA 4.0** | `CC-BY-SA-4.0` | [`cc-by-sa-4.0.md`](cc-by-sa-4.0.md) | Copyleft for creative works, wikis & documentation |
| **ODbL 1.0** | `ODbL-1.0` | [`odbl-1.0.md`](odbl-1.0.md) | Copyleft for structured data & databases |

---

## Archived Licenses

Deprecated, superseded, or legacy licenses (e.g. Artistic 2.0, BSD 4-Clause, CC-BY-SA 3.0, EPL 1.0, GFDL 1.3, GPL 1.0, MS-PL) are preserved in [`archive/`](archive/README.md). They remain available for historical reference but are not recommended for new projects.

---

## Usage

1. Choose a license that fits your project requirements.
2. Copy the corresponding `.md` file to your repository as `LICENSE.md` (or `LICENSE`).
3. Fill in the placeholder fields (such as copyright year and owner).
