# Company Data Extraction

Automated CNPJ data pipeline · Python · Selenium · Excel

---

## Overview

Desktop application that automates the retrieval of publicly available company data from Brazilian government sources using CNPJ identifiers. Built to demonstrate real-world automation and data pipeline patterns applicable to industrial data acquisition and IoT backend workflows.

---

## Technical Highlights

**Automated data acquisition**
Selenium-driven web scraping pipeline with robust error handling and retry logic — mirroring sensor polling patterns in IoT systems.

**Concurrent batch processing**
Multi-threaded architecture allows simultaneous CNPJ lookups, keeping the UI responsive while background workers process data. Pattern reusable for parallel device communication in edge systems.

**Structured data output**
Extraction results are normalized and written to Excel (.xlsx), enforcing a consistent schema regardless of source variability — the same concern found in industrial data historians and SCADA data export pipelines.

**Desktop GUI (PySimpleGUI)**
Cross-platform interface targeting both Windows and macOS, with non-blocking feedback and progress reporting during long-running operations.

---

## Stack

Python 3.x · PySimpleGUI · Selenium · openpyxl · threading

---

## Installation

```bash
git clone https://github.com/Phernando82/busca_empresa.git
cd company-data-extraction
pip install -r requirements.txt
python main.py
```

---

## Usage

1. Enter one or more CNPJ numbers (one per line)
2. Click **Start** — background threads begin fetching data
3. Monitor progress in the status panel
4. Export result to Excel when complete

---

## Relevance to Industry 4.0

The patterns demonstrated here — automated data acquisition, concurrent worker threads, schema-enforced structured output, and cross-platform desktop delivery — map directly to common requirements in industrial IoT: polling remote endpoints, aggregating heterogeneous data sources, and producing reports for MES/ERP integration.

---

## License

MIT · Data sourced exclusively from public government registries.  
No private or sensitive information is accessed or stored.
