# cycov-home-assistant

An aggregation repository that holds Home Assistant add-ons, HACS Lovelace cards, and custom components. Each sub-project is managed as a **git subtree** sourced from its own upstream GitHub repository.

## Repository Structure

```
cycov-home-assistant/
├── addons/              # Home Assistant add-ons
├── custom_components/   # Custom integrations / components
└── www/                 # HACS Lovelace cards & frontend resources
```

## Git Subtree Workflow

### Add a new subtree

```bash
git subtree add --prefix=<path>/<name> <remote-url> <branch> --squash
```

**Examples:**

```bash
# Add a new add-on
git subtree add --prefix=addons/my-addon https://github.com/user/my-addon main --squash

# Add a custom component
git subtree add --prefix=custom_components/my-component https://github.com/user/my-component main --squash

# Add a Lovelace card
git subtree add --prefix=www/my-card https://github.com/user/my-card main --squash
```

### Update an existing subtree

```bash
git subtree pull --prefix=<path>/<name> <remote-url> <branch> --squash
```

### Push local changes back to the upstream subtree

```bash
git subtree push --prefix=<path>/<name> <remote-url> <branch>
```

## Sections

| Directory | Contents |
|-----------|----------|
| [`addons/`](addons/) | Home Assistant supervisor add-ons |
| [`custom_components/`](custom_components/) | Custom integrations loaded by Home Assistant |
| [`www/`](www/) | Lovelace cards and other frontend resources (HACS) |

See the `README.md` inside each directory for the list of included subtrees and per-section subtree commands.
