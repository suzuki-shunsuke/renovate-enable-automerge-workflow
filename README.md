# renovate-enable-automerge-workflow

GitHub Actions Reusable Workflow to enable automerge of a pull request from Renovate

## How to use

```yaml
---
name: test
on:
  pull_request: {}
permissions: {}
jobs:
  enable-automerge:
    uses: suzuki-shunsuke/renovate-enable-automerge-workflow/.github/workflows/enable_automerge.yaml@main
    secrets:
      gh_app_id: ${{secrets.GH_APP_ID}}
      gh_app_private_key: ${{secrets.GH_APP_PRIVATE_KEY}}
    permissions: {}
```

## Workflow

[Workflow](.github/workflows/enable_automerge.yaml)

## Requirements

- GitHub CLI

GitHub Personal Access Token or GitHub App

permissions

- contents: write
- pull-requests: write

## LICENSE

[MIT](LICENSE)
