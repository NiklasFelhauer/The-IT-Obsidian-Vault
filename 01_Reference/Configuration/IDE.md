
## VS Code

### settings.json (black and isort on save)

```python

{
    "git.autofetch": true,
    "editor.minimap.enabled": false,
    "explorer.confirmDragAndDrop": false,
    "security.workspace.trust.untrustedFiles": "open",
    "[json]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "liveServer.settings.proxy": {
        "enable": true,
        "baseUri": "/",
        "proxyUri": "http://localhost:4200"
    },
    "liveServer.settings.port": 4200,
    "liveServer.settings.donotShowInfoMsg": true,
    "git.openRepositoryInParentFolders": "never",
    "git.confirmSync": false,
    "explorer.confirmDelete": false,
    "terminal.integrated.enableMultiLinePasteWarning": false,
    "javascript.updateImportsOnFileMove.enabled": "always",
    "git.ignoreRebaseWarning": true,
    "docker.extension.enableComposeLanguageServer": false,
    "github.copilot.nextEditSuggestions.enabled": true,
    "docker.extension.dockerEngineAvailabilityPrompt": false,
    "sonarlint.focusOnNewCode": false,
    "[python]": {
        "editor.defaultFormatter": "ms-python.black-formatter",
        "editor.formatOnSave": true
    },
    "editor.codeActionsOnSave": {
        "source.organizeImports": "explicit"
    },
    "isort.args": ["--profile", "black"],
    "black-formatter.args": ["--line-length", "88"]
}

```

