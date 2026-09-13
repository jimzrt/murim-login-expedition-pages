# Murim Login — Chapter 374 Expedition Pages

This repository is the deployment shell for the temporary Chapter 374
expedition reader. It checks out the source repository's
`expedition/chapter-374` branch when it receives the `expedition-publish`
repository-dispatch event, builds the Astro reader, and deploys it to GitHub
Pages.

The source content and translation workflow live in
[jimzrt/murim-login](https://github.com/jimzrt/murim-login). The expedition
intentionally skips Chapters 65–373; the reader displays that boundary.

In repository settings, configure **Pages → Build and deployment → Source:
GitHub Actions**. The source repository must have an `EXPEDITION_PAGES_TOKEN`
secret that can dispatch workflows in this repository.
