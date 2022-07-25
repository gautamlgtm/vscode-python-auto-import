# Python Auto Importer

## Setup

### Installing the extension

```bash
npm install -g vsce

npm install --save-dev webpack-cli # Install webpack plugin if you don't already have it installed
npm install webpack # Install this if you still get errors

vsce package  # This step will output a path to a vsix file
code --install-extension <path-to-vsix>
```

### Extension setup

Create a new Python 3.10 virtualenv.

```bash
python3.10 -m venv <path-to-venv>
```

In your vscode `settings.json` set `python-auto-importer.pythonInterpreterPath` to the virtualenv's python.

## Key bindings

Fix imports for a file: `Cmd + Shift + I`
