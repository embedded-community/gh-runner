# gh-runner
Github CLI extension for managing github self-hosted action runners

## Installation

```bash
gh extension install embedded-community/gh-runner
```

```bash
pip install -r requirements.txt
```

## Usage

Define organization with either `GH_RUNNER_EXTENSION_GITHUB_ORGANIZATION` env variable or giving
`gh runner --org <github-organization>` parameter for each command execution.



### List organization runner groups

```bash
$ gh runner groups --help
usage: gh-runner groups [-h] {list} ...

optional arguments:
  -h, --help  show this help message and exit

Groups subcommands:
  {list}
    list      List all groups
```

### Show runner group details

```bash
$ gh runner group show --help
usage: gh-runner group show [-h] group_id {repos,runners,all}

positional arguments:
  group_id             Group ID
  {repos,runners,all}  Info type, one of repos|runners|all

optional arguments:
  -h, --help           show this help message and exit
```
