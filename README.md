# Obsidian Calendar Test: information website

A static information website for the OAuth application. Includes a home page, Privacy Policy and Terms of Use. It does not perform authorization or receive calendar data.

## Local build

Install [Zola 0.23.6](https://github.com/getzola/zola/releases/tag/v0.23.6), then run these commands from the repository root:

```sh
zola check --skip-external-links
zola build
zola serve
```

For a different address, use `zola build --base-url https://YOUR-USER.github.io/YOUR-REPOSITORY/`. Page and stylesheet links respect the project's URL subpath.

## GitHub Pages

Under Settings > Pages, select GitHub Actions as the source. The workflow builds the site with a pinned Zola version and publishes only `public/`. The Zola archive is verified against its SHA-256 checksum, and Actions are pinned to full commit identifiers. No additional secrets are required.

The public repository must contain only this website's source files. Do not add an Obsidian vault, plugin settings, OAuth parameters, tokens, logs or images containing personal information. Technical checks and setup evidence are not part of the website.

The policy's date and contents must match the actual connection configuration. Publishing this website does not move the OAuth application to Production or confirm Google verification.
