# python-code-visualiser
## Overview

Python Code Visualiser is a github action that will create mermaid class diagrams of the a repo.  The diagram can be posted to a PR as a comment to assist with Code Review, or just add as an artifact.

The repo makes use of the fantastic [pymermaider](https://github.com/diceroll123/pymermaider) to create the diagrams.

## Usage
### Permission

The following workflow permissions are necessary:

```yml
permissions:
  contents: read
  statuses: write
```

### Inputs

`python-code-visualiser` uses the following inputs:

| Name       | Description                                                                                                                                                                                                              | Required | Default        |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------- | -------------- |
| `gh-token` | `GITHUB_TOKEN` (permissions `contents: write` and `pull-requests: write`) or a `repo` scoped [Personal Access Token (PAT)](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token). | no       | `GITHUB_TOKEN` |

## Outputs

## Contributing

Contributions are more than welcome, just make a PR and we'll go from there!

## License

This project is licensed under the MIT license. Please see the
[LICENSE](LICENSE) file for more details.