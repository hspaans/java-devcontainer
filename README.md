# Devcontainer for Java

## Using within you project

Add `.devcontainer/devcontainer.json` to your repository.

```json
{
  "image": "ghcr.io/hspaans/java-devcontainer:latest",
  "name": "Java",
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "appPort": [8080],
  "postCreateCommand": "",
  "remoteUser": "vscode",
  "extensions": [
    "github.vscode-pull-request-github",
    "editorconfig.editorconfig",
    "vscjava.vscode-java-pack",
    "pivotal.vscode-boot-dev-pack",
    "redhat.vscode-yaml"
  ]
}
```
