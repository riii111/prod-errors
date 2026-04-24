# prod-errors

Production error triage tools for Google Cloud Error Reporting and Cloud Logging.

## Commands

- `prod-errors summary`: list current error groups
- `prod-errors trace <groupId>`: inspect one error group
- `prod-errors hotspots`: analyze error trends
- `pe`: short alias for `prod-errors`

## Install

This repository is intended to be applied as a private chezmoi source layer.

```sh
chezmoi -S . apply
```

## Test

```sh
python3 -m unittest tests.test_prod_errors
```
