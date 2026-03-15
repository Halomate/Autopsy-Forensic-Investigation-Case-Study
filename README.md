# Digital Forensics Investigation using Autopsy

## Overview

This project demonstrates a **digital forensic investigation using Autopsy**, an open-source digital forensics platform used by investigators to analyze disk images and recover digital evidence.

The objective of this investigation was to analyze a suspect workstation disk image and determine whether an employee accessed or attempted to exfiltrate proprietary company data.

This case study simulates an **insider threat investigation**, focusing on recovering deleted files, analyzing metadata artifacts, and identifying suspicious user activity.

---

## Investigation Scenario

A company suspected an employee of accessing and potentially distributing **confidential business documents** without authorization.

A forensic investigation was conducted on the employee's workstation to determine:

* Whether confidential files were accessed
* Whether deleted files could be recovered
* If evidence of data exfiltration existed
* Whether user activity suggested malicious intent

The investigation was conducted using **Autopsy** to analyze the suspect disk image.

---

## Tools Used

* **Autopsy** – Digital forensic investigation platform
* Disk Image Analysis
* File Carving
* Keyword Search
* Metadata Analysis
* Timeline Investigation

---

## Investigation Methodology

### 1. Case Creation

A new forensic case was created in Autopsy.

Steps included:

* Launching Autopsy
* Creating a new case
* Entering examiner information
* Importing the suspect disk image

This process establishes the environment for evidence analysis.

![Case_Creation](screenshots/case_creation.png)

---

### 2. Disk Image Ingestion

The suspect disk image was imported into the forensic case.

Autopsy ingest modules were used to automatically analyze artifacts including:

* File type identification
* Recent activity analysis
* Hash lookup
* Embedded file extraction
* Keyword search

These modules allow investigators to quickly identify potential evidence within the disk image.

![Disk_Image](screenshots/disk_image_ingest.png)

---

### 3. Keyword Search Investigation

Keyword searches were conducted to locate files related to sensitive business information.

Example keywords included:

* Confidential
* Proprietary
* Company-specific terminology

The search returned **multiple results associated with confidential documents** stored within the disk image.

![Keyword_Search](screenshots/keyword_search.png)

---

### 4. Deleted File Recovery

Using the **Deleted Files** filter in Autopsy, several deleted files were recovered from unallocated disk space.

Recovered documents included:

* Business_Strategy.pdf
* Drilling_Methodology.pdf
* Oil Company Data Strategy.pdf

The presence of these files in **carved and unallocated space** indicates the files had been deleted, potentially in an attempt to conceal them.

![Deleted_Files](screenshots/deleted_files_recovery.png)

---

### 5. Timeline Analysis

The Autopsy **Timeline module** was used to reconstruct user activity.

Timeline analysis allowed the investigation to identify:

* File creation timestamps
* File modification activity
* User access patterns
* Potential correlations between file activity and suspicious behavior

![Timeline_Analysis](screenshots/timeline_analysis.png)

---

## Key Findings

The forensic investigation uncovered several indicators of potential data exfiltration:

* Multiple confidential company documents were recovered from deleted disk space
* Keyword searches identified proprietary documents labeled **CONFIDENTIAL**
* Metadata artifacts confirmed the documents contained sensitive company information
* A document related to **anonymous Bitcoin transactions** was recovered near the confidential files

The presence of cryptocurrency-related documentation alongside proprietary files raises concern regarding potential plans to distribute or sell company data anonymously.

![Metadata_Evidence](screenshots/metadata_evidence.png)

---

## Conclusion

The forensic analysis revealed that the suspect had access to and deleted multiple confidential corporate documents.

Evidence recovered from the disk image suggests potential attempts to conceal or prepare proprietary data for unauthorized distribution.

These findings indicate a likely violation of the organization's **Acceptable Use Policy (AUP)** and **Nondisclosure Agreement (NDA)**.

---

## Skills Demonstrated

* Digital Forensic Investigation
* Disk Image Analysis
* Deleted File Recovery
* Metadata Analysis
* Timeline Reconstruction
* Evidence Documentation
* Incident Investigation

---

## References

National Institute of Standards and Technology (NIST).
Guide to Integrating Forensic Techniques into Incident Response (SP 800-86)

Guide to Computer Forensics and Investigations – Nelson, Phillips, & Steuart

---

## Author

Caleb Espinoza
