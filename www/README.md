# www (HACS Lovelace Cards & Frontend Resources)

This directory contains custom Lovelace cards and other frontend resources managed as git subtrees.

Place this directory (or its contents) under your Home Assistant `config/www/` folder so that
resources are available to Lovelace. Register each resource in your Lovelace configuration.

## Adding a new Lovelace card subtree

```bash
git subtree add --prefix=www/<card-name> <remote-url> <branch> --squash
```

## Updating an existing Lovelace card subtree

```bash
git subtree pull --prefix=www/<card-name> <remote-url> <branch> --squash
```

## Available Lovelace Cards / Frontend Resources

| Resource | Source Repository | Description |
|----------|-------------------|-------------|
| *(none yet)* | — | — |
