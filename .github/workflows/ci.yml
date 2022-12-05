name: ci
on:
  push:
    branches:
      - main
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2.5.0
      - uses: actions/setup-python@v2.3.3
      - run: pip install mkdocs-material
      - run: pip install mkdocs-roamlinks-plugin
      - run: pip install mkdocs-mermaid2-plugin
      - run: mkdocs gh-deploy --force
