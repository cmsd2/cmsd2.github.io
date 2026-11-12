# cmsd2.github.io

Home page, built with [Zola](https://www.getzola.org/) and deployed to GitHub
Pages by `.github/workflows/pages.yml` on every push to `master`.

```sh
brew install zola
zola serve          # http://127.0.0.1:1111, live reload
zola build          # writes public/
```

- `content/_index.md`: the home page text
- `data/projects.toml`: rows of the Projects table
- `config.toml` `[extra]`: location, GitHub, email (shown obfuscated), photo
- `templates/`, `static/style.css`: layout and styling

The footer's "Last modified" uses the last commit time in CI (`LAST_MODIFIED`)
and falls back to build time locally.
