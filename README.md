# infra-charts

Personal shared Helm charts for feature environments.

## Charts

- `charts/mysql`: lightweight MySQL 5.7.44 chart for shared or PR environments
- `charts/redis`: copied from the current internal redis chart to keep the version aligned

## Publish

This repository is prepared for GitHub Pages + `chart-releaser-action`.

After the first push:

1. Enable GitHub Pages for this repository
2. Use branch `gh-pages` as the Pages source

Then the chart repository URL will be:

```text
https://elioncode.github.io/infra-charts
```

## Example

```bash
helm repo add infra-charts https://elioncode.github.io/infra-charts
helm repo update
```

