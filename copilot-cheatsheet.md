** Github Copilot + Copilot Chat + VSCode **

---

## 🧠 GitHub Copilot Modes (Quick Reference)

| Mode      | Description                                                                   |
| --------- | ----------------------------------------------------------------------------- |
| **Ask**   | Natural language Q\&A. Ask questions about your code, libraries, errors, etc. |
| **Edit**  | Modify selected code using a prompt (e.g., “convert to async” or “optimize”). |
| **Agent** | Structured task execution, often triggered by `/`, `@`, or `#` commands.      |

---

## 💬 Slash `/` Commands

| Command           | Description                                     |
| ----------------- | ----------------------------------------------- |
| `/search`         | Search codebase for references or symbols       |
| `/startDebugging` | Starts the VSCode debugger                      |
| `/explain`        | Explains selected code or output                |
| `/fix`            | Attempts to fix highlighted code or error       |
| `/new`            | Creates new code based on your prompt           |
| `/newNotebook`    | Creates a new Jupyter notebook                  |
| `/setupTests`     | Helps set up tests for the selected code/module |
| `/tests`          | Generates tests for selected functions or files |

---

## 🧠 `@` Agent Invocation

| Command              | Description                                                                 |
| -------------------- | --------------------------------------------------------------------------- |
| `@terminal`          | Applies the command or prompt to the terminal context                       |
| `@vscode`            | Applies within the general VSCode environment                               |
| `@workspace`         | Applies across the entire project or workspace                              |
| `@terminal /explain` | Explains the last output in the terminal                                    |
| `@workspace /fix`    | Attempts to detect and fix issues across the entire workspace               |
| `@workspace /tests`  | Suggests test cases for the selected file, function, or module project-wide |

---

## 🧩 Hash `#` Tags (Entities/References)

| Tag                    | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| `#changes`             | Shows recent changes or diffs                         |
| `#codebase`            | Refers to the entire codebase                         |
| `#extensions`          | Targets extensions installed in VSCode                |
| `#fetch`               | References fetch requests or usage in code            |
| `#findTestFiles`       | Lists or references test files                        |
| `#githubRepo`          | Refers to GitHub repository context                   |
| `#newJupyterNotebook`  | Create new Jupyter notebook                           |
| `#openSimpleBrowser`   | Opens a simple browser instance in VSCode             |
| `#problems`            | Shows problems panel (errors/warnings)                |
| `#runCell`             | Runs a cell in a notebook                             |
| `#searchResults`       | Targets the results from a previous code search       |
| `#terminalLastCommand` | Uses output or result of last terminal command        |
| `#terminalSelection`   | Uses currently selected terminal output               |
| `#testFailure`         | Points to failed tests                                |
| `#usages`              | Shows where a variable/function is used               |
| `#vscodeAPI`           | Targets VSCode extension or API-related documentation |

---

## VSCode Settings.json in regards to co-pilot

``` json
{
  // VS Code Telemetry Settings
  "telemetry.enableTelemetry": false,
  "telemetry.enableCrashReporter": false,

  // GitHub Copilot Core Settings
  "github.copilot.enable": true,
  "github.copilot.inlineSuggest.enable": true,
  "github.copilot.editor.enableAutoCompletions": true,

  // Control public code suggestions (turn off to avoid licensing/duplication issues)
  "github.copilot.advanced": {
    "suggestionMatchingPublicCode": false
  },

  // Chat-related settings
  "github.copilot.chat.enable": true, // set to false to completely disable chat
  "github.copilot.chat.showInEditor": true,
  "github.copilot.chat.showToolbar": true,

  // Allow/disallow specific languages
  "github.copilot.languages": {
    "plaintext": false,
    "markdown": false,
    "javascript": true,
    "python": true,
    "json": true
  },

  // Copilot feedback (set to false to avoid sending training data)
  "github.copilot.enableFeedback": false,

  // Optional UI Preferences
  "editor.suggest.showWords": true,
  "editor.suggestSelection": "recentlyUsedByPrefix",
  "editor.inlineSuggest.enabled": true,

  // Hide Copilot from status bar if desired
  "github.copilot.statusBar.enabled": true // set to false to hide
}
```

- Generate server side code with express.js
- scan for vulnerabilites across entire codebase
- create quiz based on entire codebase, can select specific files, ignore readme.md, test, etc. Or just to learn the codebase of a git repo.
- dummy data, list of 20 employees with whatever keys in valid json format
- @vscode cam change to dark theme, ai for settings.json
- when creating comments use pseudocode instead of prompt like requests