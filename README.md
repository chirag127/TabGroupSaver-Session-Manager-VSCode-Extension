# TabGroupSaver Session Manager VSCode Extension

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension/ci.yml?branch=main&style=flat-square)](https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension/actions)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension?style=flat-square)](https://app.codecov.io/gh/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension)
[![Tech Stack](https://img.shields.io/badge/Tech-Typescript%20%7C%20VS%20Code%20Extension-blue?style=flat-square)](https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension)
[![Lint](https://img.shields.io/badge/Lint-Biome-60c?style=flat-square)](https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square)](https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension/blob/main/LICENSE)
[![Stars](https://img.shields.io/github/stars/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension?style=flat-square)](https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension/stargazers)

---

## 🎯 Quick Value Proposition (BLUF)
Save, restore, and organize groups of VS Code tabs as named sessions—boosting focus and workflow continuity. Auto‑save, default groups, and scoped storage make session management effortless for developers of any size.

---

## 📂 Repository Architecture
text
TabGroupSaver-Session-Manager-VSCode-Extension/
├─ .github/
│  └─ workflows/ci.yml
├─ src/
│  ├─ commands/          # VS Code command implementations
│  ├─ services/          # Session persistence & auto‑save logic
│  └─ utils/             # Helper utilities
├─ tests/
│  └─ *.test.ts         # Vitest unit & integration tests
├─ scripts/
│  └─ build.ts          # Build automation
├─ package.json
├─ biome.json
├─ tsconfig.json
└─ README.md

*Feature‑Sliced Design (FSD) applied at the `src/` level for clear separation of concerns.*

---

## 📑 Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [AI Agent Directives](#ai-agent-directives)
- [Contributing](#contributing)
- [License](#license)

---

## 🚀 Installation
bash
# Clone the repository
git clone https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension.git
cd TabGroupSaver-Session-Manager-VSCode-Extension

# Install dependencies (uses npm; compatible with pnpm/yarn)
npm ci


## 🛠️ Usage
1. Open VS Code and press <kbd>Ctrl+Shift+P</kbd>.
2. Run **"TabGroupSaver: Save Current Session"** to capture the active tab set.
3. Retrieve saved sessions via **"TabGroupSaver: Restore Session"**.
4. Configure default groups and storage scopes in the extension settings (`File → Preferences → Settings → TabGroupSaver`).

---

## 📦 Development Standards
### Scripts
| Script | Description |
|--------|-------------|
| `npm run lint` | Run Biome linter (auto‑fix enabled). |
| `npm run test` | Execute Vitest suite with coverage. |
| `npm run build` | Compile the extension (`vsce package`). |
| `npm run watch` | Watch source files and rebuild on change. |

### Principles
- **SOLID**: Each service adheres to single responsibility and dependency inversion.
- **DRY**: Shared utilities live under `src/utils/`.
- **YAGNI**: Features are added only when a concrete need is identified.

### Verification Commands
bash
npm run lint        # Lint & format
npm run test        # Unit & integration tests
npm run build       # Build VSIX package

All CI checks mirror these commands to guarantee consistency.

---

## 🤖 AI Agent Directives
<details>
<summary>Expand to view agent directives</summary>

### Core Identity & Prime Directive
- **Role**: Apex Technical Authority – deliver zero‑defect, high‑velocity VS Code extension.
- **Mission**: Enable developers to persist and restore workspace states instantly.

### Tech Stack
- **Language**: TypeScript (strict mode).
- **Package Manager**: npm (compatible with pnpm/yarn).
- **Linter/Formatter**: Biome.
- **Testing**: Vitest (unit & integration), with coverage reported to Codecov.
- **Build**: VS Code Extension (`vsce`).

### Architectural Patterns
- **Feature‑Sliced Design (FSD)** – logical grouping of commands, services, and utilities.
- **Hexagonal/Ports‑&‑Adapters** – `services/` act as core domain, `extension/` as adapters.
- **SOLID**, **DRY**, **YAGNI** enforced throughout.

### Verification / CI Commands
bash
# Lint & auto‑fix
npm run lint

# Test with coverage
npm run test

# Build VSIX package
npm run build

The CI workflow (`.github/workflows/ci.yml`) runs the above in sequence on every push and pull request.

### Continuous Improvement Loop
1. **Monitor**: Badge status & coverage metrics.
2. **Analyze**: On failure, auto‑trigger a re‑run with increased concurrency (max 5 workers).
3. **Heal**: Agents may suggest patches; PRs must pass all checks before merge.

</details>

---

## 🤝 Contributing
Please read the [CONTRIBUTING.md](https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension/blob/main/CONTRIBUTING.md) for guidelines on how to propose enhancements, report bugs, and submit pull requests.

---

## 📄 License
This project is licensed under the **Creative Commons Attribution‑NonCommercial 4.0 International (CC BY‑NC 4.0)**. See the [LICENSE](https://github.com/chirag127/TabGroupSaver-Session-Manager-VSCode-Extension/blob/main/LICENSE) file for details.
