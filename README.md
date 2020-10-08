![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/proum-public/actions/Lint/main)

# Proum-Public GitHub Actions

> This repository provides GitHub Actions that help to increase the quality of your repositories

# Usage

```yaml
jobs:
  lint:
    name: Lint repository content
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repo
        uses: actions/checkout@v2
      - name: Lint Markdown
        uses: proum-public/actions/lint/markdown@main
      - name: Lint YAML
        uses: proum-public/actions/lint/yaml@main
      - name: Lint Dockerfile
        uses: proum-public/actions/lint/dockerfile@main
        with:
          dockerfile: Dockerfile
```

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available,
see the [tags on this repository](https://github.com/your/repository/tags).

## License

This project is licensed under the GNU v2 License -
see the [LICENSE.md](LICENSE.md) file for details.