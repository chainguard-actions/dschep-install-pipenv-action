# Github Action to install pipenv

<p align="left">
  <a href="https://github.com/dschep/install-pipenv-action"><img alt="GitHub Actions status" src="https://github.com/dschep/install-pipenv-action/workflows/PR%20Checks/badge.svg"></a>
</p>

This action sets up a pipenv for use in actions by:

- installing a version of pipenv with your configured version of python

# Usage

See [action.yml](action.yml)

Basic:
```yaml
steps:
- uses: actions/checkout@master
- uses: actions/setup-python@v1
- uses: actions/pipenv@v1
- run: pipenv run my_script.py
```

With a specific version:
```yaml
- uses: actions/pipenv@v1
  with:
    version: 2018.11.26
```

# License

The scripts and documentation in this project are released under the [MIT License](LICENSE)

# Contributions

Contributions are welcome!  See [Contributor's Guide](docs/contributors.md)

## Privacy

This Action contacts Chainguard's licensing server to verify authorization. Connection metadata (IP address, GitHub repository identifier, timestamp, and any metadata encoded in the auth token) is transmitted to Chainguard, Inc. even if authorization is denied in accordance with our [Privacy Notice](https://www.chainguard.dev/legal/privacy-notice)
