# swift-repl

swift-repl is a super-fast environment for exploring and experimenting with Swift on your local machine. Designed to run seamlessly within VSCode, it enables quick feedback and smooth experimentation.

## Features

- Lightning-fast execution: Runs Swift code instantly without the need for compilation.
- Local integration: Designed to work directly within VSCode, leveraging your local setup.
- Simple and lightweight: A minimal yet powerful setup for experimenting with Swift.

## Installation

### Prerequisites

- Install [Swift](https://www.swift.org/install)
- Install [VSCode](https://code.visualstudio.com/download)

### Install recommended extensions

The workspace includes a list of suggested extensions to enhance your development experience. When you open the project in VSCode, it will prompt you to install these recommended extensions.

If the notification doesn't show up you can manually open up Recommended Extensions settings as follows:

- Open the command palette CMD + Shift + p
- Type Show Recommended Extensions

All the extensions can be installed together or only required extensions can be installed.

The following extensions are suggested:

- Swift (swiftlang.swift-vscode) - Swift Language Support for Visual Studio Code.

- Error Lens (usernamehw.errorlens) – Highlights errors and warnings directly in your code.

### Keybindings

To achieve functionality similar to Replit, add these entries to your keybindings.json file.

```json

[
  {
    "key": "cmd+enter",
    "command": "workbench.action.tasks.runTask",
    "args": "build",
    "when": "editorTextFocus && (editorLangId == 'swift' || editorLangId == 'typescript') && config.workspaceKeybindings.repl.enabled"
  },
  {
    "key": "cmd+enter",
    "command": "workbench.action.tasks.terminate",
    "args": "terminateAll",
    "when": "taskRunning && editorTextFocus && (editorLangId == 'swift' || editorLangId == 'typescript') && config.workspaceKeybindings.repl.enabled"
  }
]
```

## Usage

1. Open the project in VSCode.

2. Start experimenting with Swift syntax and features.

3. Update results on demand with Command+Enter, similar to Replit.

## Contributing

We welcome contributions! If you have ideas for new features, improvements, or bug fixes, feel free to open an issue or submit a pull request.
