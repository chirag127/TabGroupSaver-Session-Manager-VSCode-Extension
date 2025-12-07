# CodeSense-Tab-Group-Manager-VSCode-Extension

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension/ci.yml?style=flat-square&logo=github)](https://github.com/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension?style=flat-square&logo=codecov)](https://codecov.io/gh/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension)
[![License](https://img.shields.io/github/license/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension?style=flat-square)](LICENSE)
[![VSCode Version](https://img.shields.io/badge/VSCode-1.85%2B-blue?style=flat-square&logo=visualstudiocode)](https://code.visualstudio.com/)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension?style=flat-square)](https://github.com/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension)

**Star ⭐ this Repo to follow cutting-edge development!**

## BLUF: Value Proposition

**CodeSense Tab Group Manager** is an elite VS Code extension engineered to eliminate context switching overhead by providing robust, persistent management for tab groups across all your development sessions. It ensures immediate state restoration, leveraging TypeScript for high reliability and performance within the editor ecosystem.

## Architecture Overview

This extension follows a layered architecture standard, prioritizing decoupling between the UI/Editor Interaction Layer and the Persistence/Storage Layer. This adheres to SOLID principles, specifically the Dependency Inversion Principle, allowing for future storage adapters (e.g., cloud sync).

text
.CodeSense-Tab-Group-Manager-VSCode-Extension
├── src/
│   ├── editor/       // VSCode API Interaction (Views, Commands)
│   ├── storage/      // Abstraction layer for persistence (Workspace/Global/File)
│   └── core/         // Business logic: Grouping, Saving, Restoring
├── package.json      // Manifest & Dependencies (TypeScript, WXT Framework)
└── tsconfig.json


## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [Usage Guide](#usage-guide)
4. [Development & Contributing](#development--contributing)
5. [🤖 AI Agent Directives](#-ai-agent-directives)
6. [License](#license)

## Features

*   **Persistent Session Saving:** Automatically or manually save complex tab group arrangements. 
*   **Workspace Scoping:** Choose to store session definitions globally, per-workspace, or file-specific. 
*   **Instant Restore:** Re-open saved sessions with a single command, restoring layout and focus instantly.
*   **High Reliability:** Built entirely on modern **TypeScript** with strict configuration to prevent runtime errors common in extensions.
*   **Workflow Automation:** Seamlessly integrates into existing VS Code commands and keybindings for zero-friction adoption.

## Installation

1.  Open Visual Studio Code.
2.  Navigate to the Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X`).
3.  Search for `CodeSense Tab Group Manager`.
4.  Click **Install**.

Alternatively, install directly from the Marketplace link (once published).

## Usage Guide

### Saving a Session

1.  Arrange your current tab groups as desired.
2.  Open the Command Palette (`Ctrl+Shift+P`).
3.  Execute: `CodeSense: Save Current Session`.
4.  Provide a unique name for the session.

### Restoring a Session

1.  Open the Command Palette (`Ctrl+Shift+P`).
2.  Execute: `CodeSense: Restore Session By Name`.
3.  Select the desired session from the list.

### Configuration

Adjust default storage location (Global/Workspace) in VS Code Settings (`settings.json`).

---

## Development & Contributing

We adhere to the **Apex Technical Authority** standards. Contributions must be high-quality, well-tested, and follow the established architecture (SOLID, DRY).

### Setup

1.  **Clone:** `git clone https://github.com/chirag127/CodeSense-Tab-Group-Manager-VSCode-Extension.git`
2.  **Navigate:** `cd CodeSense-Tab-Group-Manager-VSCode-Extension`
3.  **Dependencies (Using uv/npm equivalents for TypeScript tooling):** `npm install` (or `pnpm install`)
4.  **Compile & Watch:** `npm run dev`
5.  **Test Locally:** Use the VS Code Extension Host debugger.

### Scripts

| Script | Command | Description |
| :--- | :--- | :--- |
| `build` | `npm run build` | Compiles TypeScript to JavaScript. |
| `watch` | `npm run watch` | Compiles and watches for changes. |
| `test` | `npm run test` | Runs Vitest unit tests. |
| `lint` | `npm run lint` | Checks code quality using Biome. |

### Guiding Principles

*   **SOLID:** Dependencies must be explicitly managed.
*   **DRY:** Avoid redundant logic, especially around VS Code API calls.
*   **YAGNI:** Only implement features required for current scope; avoid premature abstraction.

---

## 🤖 AI Agent Directives

<details>
  <summary>Apex Agent Configuration (December 2025)</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard. The project is a **TypeScript/Vite VS Code Extension**.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs. Always confirm VS Code Extension APIs via official documentation.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **VS Code Extension API Updates (v2026)**, and **State Management Best Practices for Extensions**.
    *   **Validation:** Use `docfork` to verify *every* external API signature (especially storage mechanisms).
    *   **Reasoning:** Engage `clear-thought-two` to architect complex state synchronization flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x (Strict Mode)**, **Vite 7 (Rolldown)**, and the **WXT Framework** for modern extension scaffolding. **Biome** is used for linting/formatting, and **Vitest** for unit testing. **Playwright** handles E2E verification.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)** principles adapted for VS Code extensions, ensuring clean separation between `features`, `entities`, and `shared` state logic.
    *   **State Management:** Prioritize the use of VS Code's built-in `Memento` API for persistence layers, ensuring data survives updates gracefully. External configuration must be managed via immutable structures.
    *   **Verification Commands:** Unit tests (`npm run test`) must cover persistence serialization/deserialization logic with 95%+ coverage.

</details>

## License

This repository is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**.

See the [LICENSE](LICENSE) file for full details.
