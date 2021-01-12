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

## Versions

The container is based on [LTS](https://en.wikipedia.org/wiki/Long-term_support) distribution versions with official support and fall within N and N-1. The *latest*-tag is an experimental tag to test future releases.

| Platform | Version | Image |
|:--------:|:-------:|:-----:|
| OpenJDK  | 11      | [hspaans/java-devcontainer:11][java-devcontainer:11]         |
| OpenJDK  | 15      | [hspaans/java-devcontainer:latest][java-devcontainer:latest] |

[java-devcontainer:latest]: ghcr.io/hspaans/java-devcontainer:latest
[java-devcontainer:11]: ghcr.io/hspaans/java-devcontainer:11
