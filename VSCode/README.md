# VSCode Settings 🔧

## 📝 General

[settings.json](settings.json)

### Linting

If there's one thing you can do it is automatically apply linting.

Assumes you have ESLint installed (dbaeumer.vscode-eslint) and have NOT installed Prettier (let ESLint do this).

``` json
  //
  //
  // ESLint and code style preferences:
  //
  // Allow formatting on save
  "editor.formatOnSave": false,
  "[javascript]": {
    "editor.formatOnSave": false
  },
  "[vue]": {
    "editor.formatOnSave": false
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  // Personal preferences:
  // "editor.formatOnType": false,
  // "editor.formatOnPaste": false,
  "javascript.validate.enable": false,
  //
  // Tab size:
  "editor.tabSize": 2,
  //
  // Markdown Lint:
  "markdownlint.config": {
    "default": true,
    "MD007": false,
    "MD024": false,
    "MD036": false
  },
  // END Lint
```

## 🧩 Extensions

## ✂️ JavaScript Snippets

## ⌨️ Keyboard Shortcuts

[keybindings.json](keybindings.json)

### Testing Workflow

If there's a second thing you can do it is develop a strong testing workflow:

1. When you create a new test file, add a script for it in `package.json`
2. Edit the test file side-by-side with the main file
3. The first time you run a test, hit command-shift-enter to chose the test you are editing (under npm tasks)
4. Next time you run a test, hit command-enter to re-run the last test

Bonus: Install the Jest extension (orta.vscode-jest)

``` json
  // Choose a task to run:
  {
    "key": "shift+cmd+enter",
    "command": "workbench.action.tasks.runTask"
  },
  // Re-run the last task
  {
    "key": "cmd+enter",
    "command": "workbench.action.tasks.reRunTask"
  },
```

## ⏩ Multi-command

## ☑️ Tasks

[tasks.json](tasks.json)