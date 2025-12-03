# Drime Cloud Security Analysis & Lies

**Status:** 🔴 Archived/Final. Drime failed to respond  
**Date:** December 2025

Drime is breaking the laws for **Deceptive Commercial Practices**, **Fraud**, breaking multiple **GDPR Violations**(specifically Transparency, Integrity, Confidentiality, and misrepresentation of 'Military-Grade' security measures), and  **EU Digital Content Directive**.

## Summary
This repository contains a detailed technical investigation into **Drime Cloud** and their "Vault", "E2EE" & "Zero-Knowledge" feature(s).  
Contrary to their marketing claims of "Zero-Knowledge" and "Military-Grade End-to-End Encryption (E2EE)", technical evidence indicates that **Drime possesses the decryption keys to user data.**  

The investigation reveals that Drime Cloud appears to be a white-labeled instance of a generic $29 PHP script ("BeDrive"), utilizing standard server-side encryption rather than client-side E2EE(which is the standard).

## Key Findings

*   **False Zero-Knowledge Claims:** API analysis proves that metadata (filenames, folder structures, sizes, MIME types) is transmitted and stored in **plaintext**.
*   **Not E2EE:** The server stores Initialization Vectors (IVs) and password verification hashes, meaning Drime holds the keys to decrypt user files. This is standard *Encryption-at-Rest*, not *End-to-End Encryption*.
*   **"BeDrive" Architecture:** The backend structure, API endpoints, and code logic match a generic file-sharing script called BeDrive that's sold on CodeCanyon for $29($59 now but $29 on sale) (https://codecanyon.net/item/bedrive-file-sharing-and-cloud-storage/12700384).
*   **Artificial Data Inflation:** Analysis of database IDs suggests Drime has artificially inflated their "regular file" counter to 482M+, while the actual "Vault" usage is approximately ~34k files.
*   **Legal Violations:** The findings suggest **MULTIPLE** serious violations of GDPR (transparency/integrity), the EU Digital Content Directive, and French consumer protection laws regarding deceptive commercial practices.

## How to Read the Report

The full report is available on Github pages

1.  **[Click here](https://freminet.github.io/drime/)**

## Conclusion
Drime Cloud has failed to address these technical discrepancies despite them claiming to have "contacted me"(which they never did, and also claimed I didn't respond? what am I supposed to respond to when you never sent me anything and you're lying about it to your own customers on Drime subreddit?). As of December 2025, Drime still continues to advertise "Zero Knowledge" features that do not exist in their technical implementation to unknowing and unsuspecting customers.

**Recommendation:** Users seeking genuine privacy or protection from server-side data breaches should **AVOID** Drime Cloud.

---

**Found anything wrong?:** Contact sylphie@tuta.io
