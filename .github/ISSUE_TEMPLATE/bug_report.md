# 🐛 Bug Report Template

Thank you for investing time to improve **TabGroupManager-VSCode-Extension**. By using this template, you ensure that we can rapidly diagnose and resolve the issue based on Apex Architectural Standards.

---

## 1. 🚨 Issue Summary (BLUF)

> *Provide a concise, high-level summary of the bug in one sentence.*

**Example:** Tab groups saved under a specific name disappear immediately upon VS Code restart.

---

## 2. 🔍 Environment Context

To ensure reproducibility, please detail the environment configuration. This aligns with our 'Zero-Defect' validation protocol.

### A. Extension Specifics

*   **Extension Version:** `<!-- e.g., 1.4.0 -->`
*   **VS Code Version:** `<!-- e.g., 1.85.1 -->`
*   **Operating System:** `<!-- e.g., Windows 11, macOS Sonoma, Ubuntu 24.04 -->`

### B. Configuration Snippet

If the issue relates to configuration, please paste the relevant lines from your `settings.json`.


// Paste relevant settings.json block here


---

## 3. 📝 Steps to Reproduce (STR)

List the exact sequence of actions required to trigger this behavior. Be precise.

1.  [Action 1]
2.  [Action 2]
3.  [Action 3]
4.  ...

---

## 4. 💥 Expected vs. Actual Behavior

*   **Expected Behavior:** What should have happened according to the design specification?

*   **Actual Behavior:** What actually happened (the bug)?

---

## 5. 👁️ Logs and Artifacts

To assist debugging, please provide diagnostic output. For VS Code extensions, this typically means the **Developer Tools Console** output.

1.  Open the Developer Tools (`Help > Toggle Developer Tools`).
2.  Navigate to the **Console** tab.
3.  Reproduce the bug.
4.  Copy the complete error messages (especially those marked `ERROR` or `WARN`) below.

bash
// Paste Console Output Here


## 6. Supporting Media (Optional but Encouraged)

If applicable, include screenshots or a short screen recording demonstrating the failure state. You can link to external hosting like Loom or Imgur if the file size is large.

---

## 7. Replication Confirmation

Have you confirmed this issue persists after restarting VS Code and trying on a fresh workspace?

- [ ] Yes
- [ ] No

*Note: Issues not reproducible after environment reset may be closed until further information is provided, adhering to our efficiency mandates.*