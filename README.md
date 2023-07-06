# Software Engineering for Scientists (SE4Sci) Hack-a-thon 1 Project Solution

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python](https://img.shields.io/badge/Language-Python-blue.svg)](https://python.org/)

This is one solution to SE4Sci Hackathon 1 for groups that didn't complete the hackathon or want a fresh start.

## Overview

This repo contains a PostgreSQL model and REST API for a Fire Incident service. It can be used by any of the groups but especially those groups that did not complete Hackathon 1. You can use this is the code to start Hackathon 2.

## Automatic Setup

The best way to use this repo is to start your own repo using it as a git template. To do this just press the green **Use this template** button in GitHub and this will become the source for your repository.

## Contents

The project contains the following:

```text
.gitignore          - this will ignore vagrant and other metadata files
.flaskenv           - Environment variables to configure Flask
.gitattributes      - File to gix Windows CRLF issues
.devcontainers/     - Folder with support for VSCode Remote Containers
dot-env-example     - copy to .env to use environment variables
requirements.txt    - list if Python libraries required by your code
config.py           - configuration parameters

deploy/                    - K8s deployment files
├── deployment.yaml        - Deployment
├── postgresql.yaml        - PostgreSQL
└── service.yaml           - Service

service/                   - service python package
├── __init__.py            - package initializer
├── models.py              - module with business models
├── routes.py              - module with service routes
└── common                 - common code package
    ├── error_handlers.py  - HTTP error handling code
    ├── log_handlers.py    - logging setup code
    └── status.py          - HTTP status constants

tests/              - test cases package
├── __init__.py     - package initializer
├── factories.py    - factory classes to generate test data
├── test_models.py  - test suite for business models
└── test_routes.py  - test suite for service routes
```

## License

Licensed under the Apache License. See [LICENSE](LICENSE)

