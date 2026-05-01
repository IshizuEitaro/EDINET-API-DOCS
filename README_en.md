# EDINET API Documentation (Markdown Edition)

[Japanese Edition (README.md)](README.md)

This repository provides a cleaned, Markdown-formatted version of the "EDINET API Specification" and related documents provided by the Financial Services Agency (FSA) of Japan.

## Project Overview

This project aims to facilitate the use of corporate disclosure information by converting the original PDF documentation into Markdown. This enables "full-text search," "version control/diff management," and "integration with various developer tools" that were difficult with the original PDF format.

Beyond simple automated conversion, we have performed manual layout adjustments and integrated Mermaid diagrams to enhance the quality as technical documentation.

## Included Documents

- **[EDINET API Specification (ESE140206.md)](ESE140206.md)**
  - The main document covering API usage, endpoints, authentication, and response formats.
- **[Form Code List (ESE140327.md)](ESE140327.md)**
  - A definition list of form codes for submitted documents.
- **[Output Data Examples (ESE140328.md)](ESE140328.md)**
  - Specific examples of output data for complex use cases, such as non-disclosure processing by FSA officials.

## Reference Data

- **`EdinetcodeDlInfo.csv`**: Reference data containing EDINET codes, filer names, and securities codes.
- **`ESE140190.csv`**: Reference CSV associated with the original specification.

## Key Features and Improvements

- **Clean Markdown Format**: Manually fixed line fragmentation and table corruption often caused by PDF-to-Markdown conversion.
- **Mermaid Diagrams**: Replaced original static diagrams for document hierarchy and withdrawal flows with maintainable Mermaid.js code.
- **Optimized Tables**: Formatted large response field definitions into clean Markdown tables for better readability on GitHub.
- **Image Optimization**: Removed unused/duplicate images and consolidated necessary assets into the `ESE140206_images/` directory.

## Creation Process

1.  **Source**: Obtained the PDF from the [EDINET API Specification Page](https://disclosure2dl.edinet-fsa.go.jp/guide/static/disclosure/WZEK0110.html).
2.  **Conversion**: Generated the base Markdown using [opendataloader-pdf](https://github.com/opendataloader-project/opendataloader-pdf).
3.  **Cleanup**: Removed conversion artifacts, standardized table column orders, and fixed encoding issues.
4.  **Enhancement**: Manually implemented complex flowcharts using Mermaid.js.

## License and Disclaimer

- **Original Copyright**: The copyright of the original information belongs to the [Financial Services Agency (FSA)](https://www.fsa.go.jp/) of Japan.
- **Repository License**: The conversion process, additional structure, and diagrams in this repository are released under the [MIT License](LICENSE).
- **Compliance**: Please ensure compliance with the [EDINET Terms of Use](https://disclosure2dl.edinet-fsa.go.jp/guide/static/submit/WZEK0030.html) when using this documentation.
