# Macro-Deck-Extension-Build-Action
This repository houses the composite action for building a Macro Deck extension, plugins and icon packs. This is still a work in progress.

## How to Use
You can either use this example template as-is in a file with path `.github/workflows/build_extension.yml`, build upon it, or just use the action in your own worklow build

> **NOTE**: You can also replace `latest` with a version number (tag)

```yaml
name: Build Extension

on:
  push:
    branches: [ "main" ]
  pull_request:
    branches: [ "main" ]
  workflow_dispatch:

jobs:
  build:
  
    runs-on: ubuntu-latest

    steps:
    - name: Build Extension
      uses: RecklessBoon/Macro-Deck-Extension-Build-Action@latest
```
