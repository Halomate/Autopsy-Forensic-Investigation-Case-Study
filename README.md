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

---

### 3. Keyword Search Investigation

Keyword searches were conducted to locate files related to sensitive business information.

Example keywords included:

* Confidential
* Proprietary
* Company-specific terminology

The search returned **multiple results associated with confidential documents** stored within the disk image.

---

### 4. Deleted File Recovery

Using the **Deleted Files** filter in Autopsy, several deleted files were recovered from unallocated disk space.

Recovered documents included:

* Business_Strategy.pdf
* Drilling_Methodolog_
