# Generate CHANGELOG.md Action

Based on https://github.com/github-changelog-generator/github-changelog-generator.

## Example

```yaml
name: Generate CHANGELOG.md

on:
  push:
    tags:
      - "*"

permissions:
  contents: write

jobs:
  generate-changelog:
    runs-on: ubuntu-latest
    steps:
      - name: Generate CHANGELOG.md
        uses: ganiulis/generate-changelog-action@0.1.1
        with:
          repository-name: my-repository-name
```
