# gh-runner
Github CLI extension for managing github self-hosted action runners.

Most of the features in the extension require github enterprise.

## Installation

```bash
gh extension install embedded-community/gh-runner
```

## Usage

Define organization with either `GH_RUNNER_EXTENSION_GITHUB_ORGANIZATION` env variable or giving
`gh runner --org <github-organization>` parameter for each command execution.

Each command provides detailed help with `--help` parameter.


### List organization self-hosted runner groups

```bash
$ gh runner groups
```

### Create organization self-hosted runner group

```bash
$ gh runner groups create <name> <visibility>
```

### Show self-hosted runner group details

```bash
$ gh runner group show <group_id> <info_type>
```

### Delete self-hosted runner group

```bash
$ gh runner group delete <group_id>
```

### List organization repositories

```bash
$ gh runner repo list
```

### Link repository to self-hosted runner group

```bash
$ gh runner group manage <group_id> link-repo <repo_id>
```

### Unlink repository from self-hosted runner group

```bash
$ gh runner group manage <group_id> unlink-repo <repo_id>
```
