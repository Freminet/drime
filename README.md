# Drime Cloud Security Analysis & Lies

**Status:** 🔴 Archived/Final.
**Date:** December 2025

Drime is breaking the laws for **Deceptive Commercial Practices**, breaking multiple **GDPR Violations**(specifically Transparency, Integrity, Confidentiality, and misrepresentation of 'Military-Grade' security measures), and  **EU Digital Content Directive**.

## How to Read the Report

The full report is available on Github pages

1.  **[Click here](https://freminet.github.io/drime/)**

## Summary
This repository contains a detailed technical investigation into **Drime Cloud** and their "Vault", "E2EE" & "Zero-Knowledge" feature(s).  
Contrary to their marketing claims of "Zero-Knowledge" and "Military-Grade End-to-End Encryption (E2EE)"

The investigation reveals that Drime Cloud appears to be a white-labeled instance of a generic $29 PHP script ("BeDrive")

## Key Findings

*   **False Zero-Knowledge Claims:** API analysis proves that metadata (filenames, folder structures, sizes, MIME types) is transmitted and stored in **plaintext**.
*   **"BeDrive" Architecture:** The backend structure, API endpoints, and code logic match a generic file-sharing script called BeDrive that's sold on CodeCanyon for $29($59 now but $29 on sale) (https://codecanyon.net/item/bedrive-file-sharing-and-cloud-storage/12700384).
*   **Suspected Artificial Data Inflation:** Analysis of database IDs suggests Drime has **possibly** artificially inflated their "regular file" counter to 482M+, while the actual "Vault" usage is approximately ~34k files.
*   **Legal Violations:** The findings suggest **MULTIPLE** serious violations of GDPR (transparency/integrity), the EU Digital Content Directive, and French consumer protection laws regarding deceptive commercial practices.

## Conclusion
As of 4th December 2025, Drime still continues to advertise "Zero Knowledge" features that do not exist in their technical implementation to unknowing and unsuspecting customers.

**Recommendation:** Users seeking genuine privacy or protection from server-side data breaches should **AVOID** Drime Cloud.

---

**Found anything wrong?:** Contact sylphie@tuta.io
