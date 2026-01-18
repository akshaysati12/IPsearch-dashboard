# IPsearch-dashboard
Asset Discovery Portal is a lightweight, browser-based forensic tool designed to parse and search through massive JSON reconnaissance exports.
# Asset Discovery Portal 🔍

A high-performance, client-side web interface for searching and filtering large asset discovery JSON files.

## 🚀 Overview
When performing large-scale reconnaissance, output files can grow into the hundreds of megabytes. Opening these in standard text editors or JSON viewers is often slow or impossible. 

The **Asset Discovery Portal** solves this by:
1. **Streaming Data:** Uses `Oboe.js` to process JSON nodes as they load, preventing memory overflow.
2. **Local Processing:** Your data never leaves your machine. All indexing and filtering happen locally in your browser.
3. **Multi-Vector Filtering:** Simultaneously filter by IP, Domain, Page Title, Port, or Request type.

## ✨ Features
* **Zero-Server Architecture:** Pure HTML/JavaScript; can be hosted on GitHub Pages or run locally via `file://`.
* **Dynamic Filtering:** Add multiple filter rows to drill down into specific subnets or technologies.
* **Pagination:** Smoothly handle results sets with adjustable page sizes (100 to 1,000 records).
* **Optimized Indexing:** Specifically designed to parse common recon formats (mapping both IP and Domain-based HTTP/S responses).

## 🛠️ Installation & Usage
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/asset-discovery-portal.git](https://github.com/YOUR_USERNAME/asset-discovery-portal.git)
    ```
2.  **Open `index.html`** in any modern web browser.
3.  **Load your JSON:** Click "Choose File" and select your recon export.
4.  **Search:** Use the filter bars to find specific assets.

## 📊 Supported Data Structure
The tool is currently optimized for JSON objects containing:
* `http_responseForIP` / `https_responseForIP`
* `http_responseForDomainName` / `https_responseForDomainName`



## 🧰 Built With
* [Oboe.js](http://oboejs.com/) - For progressive streaming of JSON.
* Pure CSS - Dark mode optimized UI.
* Vanilla JavaScript - For maximum speed and zero dependencies.

## ⚖️ License
Distributed under the MIT License. See `LICENSE` for more information.
