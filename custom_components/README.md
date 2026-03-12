# Custom Components

This directory contains Home Assistant custom integrations (components) managed as git subtrees.

Place this directory inside your Home Assistant configuration directory, or symlink it there.
Home Assistant will automatically discover integrations placed under `custom_components/`.

## Adding a new custom component subtree

```bash
git subtree add --prefix=custom_components/<component-name> <remote-url> <branch> --squash
```

## Updating an existing custom component subtree

```bash
git subtree pull --prefix=custom_components/<component-name> <remote-url> <branch> --squash
```

## Available Custom Components

| Component | Source Repository | Description |
|-----------|-------------------|-------------|
| *(none yet)* | — | — |
