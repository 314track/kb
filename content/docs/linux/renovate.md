---
title: "renovate"
draft: false
---

# renovate

## create config.js

```bash
vim $HOME/.renovate/config.js
```

```json
module.exports = {
  hostRules: [
    {
      hostType: 'gitlab',
      matchHost: 'gitlab.com',
      token: '<token>',
    },
    {
      hostType: 'github',
      matchHost: 'github.com',
      token: '<token>',
    }
  ]
};
```

## Validate configuration

```bash
docker run --rm -it -e RENOVATE_CONFIG_FILE=/config.js -e LOG_LEVEL=debug -v "$(pwd)":/app -v $HOME/.renovate/config.js:/config.js renovate/renovate bash -c "git config --global --add safe.directory '*' && cd /app && renovate-config-validator"
```

## Run Renovate locally
If necessary, remove local presets in renovate.json, as they do not work with `--platform=local`.
`local>...`

TODO: Something is missing here: To be fixed

```bash
docker run --rm -it -e RENOVATE_CONFIG_FILE=/config.js -e LOG_LEVEL=debug -v "$(pwd)":/app -v $HOME/.renovate/config.js:/config.js -v .:/app renovate/renovate --platform=local --path=/app
```
