# Archived Licenses

This directory contains legacy, superseded, deprecated, or historically problematic software and content licenses.

While these licenses may still govern older codebases or historical repositories, they are **no longer recommended for new projects** as of September 2026. For active open-source projects, please select a modern license from the root directory.

---

## Overview of Archived Licenses

| License | SPDX Identifier | Status | Modern Replacement | Reason for Archival |
| :--- | :--- | :--- | :--- | :--- |
| **Artistic License 2.0** | `Artistic-2.0` | Deprecated / Legacy | [MIT](../mit.md) or [Apache-2.0](../apache-2.0.md) | Perl-specific conventions from the 1990s/2000s; rarely used in modern cross-language open source. |
| **BSD 4-Clause** | `BSD-4-Clause` | Historical / Incompatible | [BSD-3-Clause](../bsd-3-clause.md), [BSD-2-Clause](../bsd-2-clause.md), or [0BSD](../0bsd.md) | Contains the obsolete "advertising clause" (clause 3) which created attribution cascades and GPL incompatibility. |
| **Creative Commons CC-BY-SA 3.0** | `CC-BY-SA-3.0` | Superseded | [CC-BY-SA-4.0](../cc-by-sa-4.0.md) | Version 3.0 required jurisdiction-specific ports and lacked explicit provisions for sui generis database rights. |
| **Eclipse Public License 1.0** | `EPL-1.0` | Superseded | [EPL-2.0](../epl-2.0.md) | Deprecated by the Eclipse Foundation; version 2.0 adds secondary licensing compatibility (e.g. with GPL) and clarifies modern terms. |
| **GNU Free Documentation License 1.3** | `GFDL-1.3-or-later` | Deprecated for general use | [CC-BY-SA-4.0](../cc-by-sa-4.0.md) | "Invariant Sections" and cover text requirements cause compatibility issues with DFSG and modern wikis (e.g., Wikipedia transitioned away from GFDL). |
| **GNU General Public License v1.0** | `GPL-1.0-only` | Obsolete | [GPL-3.0](../gnu-gpl-v3.0.md) or [GPL-2.0](../gnu-gpl-v2.0.md) | Ancient first release from 1989; superseded by GPLv2 (1991) and GPLv3 (2007). |
| **Microsoft Public License** | `MS-PL` | Legacy | [MIT](../mit.md) or [Apache-2.0](../apache-2.0.md) | Mid-2000s CodePlex-era license; Microsoft itself transitioned all its open source initiatives to MIT and Apache-2.0. |

---

## Why Were These Moved?

1. **Ecosystem Harmonization:** Standardizing on canonical licenses (such as MIT, Apache-2.0, BSD, GPLv3, MPL-2.0, EPL-2.0) drastically reduces license compliance friction, dependency audit complexity, and SPDX scanner ambiguities.
2. **Legal Modernization:** Modern licenses (version 2.0+ or 4.0 for Creative Commons) address global jurisdiction neutrality, patent retaliation clauses, database rights, and digital network usage.
3. **Clarity for Developers:** Housing legacy licenses in a dedicated `archive/` directory prevents authors of new software from inadvertently choosing outdated or legally ambiguous terms.
