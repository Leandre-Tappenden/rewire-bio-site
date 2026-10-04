# Rewire Bio — public website

[Open Rewire Bio](https://leandre-tappenden.github.io/rewire-bio-site/)

This repository publishes the website from the `main` branch of
[nathnwe/hack-anthropic-modal-2026](https://github.com/nathnwe/hack-anthropic-modal-2026).
Make website changes in that project's `site/` directory. This repository contains
only the publishing workflow; it is not a second copy of the application source.

## Publish an update

After the source changes reach `main`, open
[Publish Rewire Bio](https://github.com/Leandre-Tappenden/rewire-bio-site/actions/workflows/pages.yml)
and select **Run workflow**, or run:

```sh
gh workflow run pages.yml --repo Leandre-Tappenden/rewire-bio-site --ref main
```

The workflow checks, tests and builds the latest source, then deploys it to the
same public URL. Its build summary records the source commit. Changes to the
source repository do not trigger this separate repository automatically.

The publishing account controls GitHub Pages here, independently of the shared
hackathon repository. The workflow needs no stored personal access token.
