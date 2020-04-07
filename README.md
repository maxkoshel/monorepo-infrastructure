# Monorepo Infrastructure

## Building with Yarn

Installing dependencies:

```bash
$ yarn
```

## Yarn Workspaces

### Adding a new workpsace

1. Define fields `version` and `name` in `package.json` of workspace.
2. Add workspace to the root `package.json` in the field `workspaces`.

### Useful receipts

Printing a full list of workspaces with their dependencies.

```bash
$ yarn workspaces info
```

Running the chosen `yarn` command in the selected workspace.

```bash
$ yarn workspace <workspace-name> <command>
```

Adding a common dependency to all packages (from the root folder).

```bash
$ yarn add <package-name> -W
```

Running script for all project packages.

```bash
$ yarn <script-name> --scope @monorepo/*
```
