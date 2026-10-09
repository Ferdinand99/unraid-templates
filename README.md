# Ferdinand99's Unraid templates

Unraid Docker templates for [Community Applications](https://ca.unraid.net).
This repository only holds the templates; each app lives in its own
repository.

| Template | App | Image |
| --- | --- | --- |
| [`templates/sylo.xml`](templates/sylo.xml) | [Sylo](https://github.com/Ferdinand99/Sylo) — multi-function Discord bot with a web dashboard | `docker.io/iwgamin/sylo` |
| [`templates/sylo-fluxer.xml`](templates/sylo-fluxer.xml) | [Sylo-Fluxer](https://github.com/Ferdinand99/Sylo-Fluxer) — Sylo ported to Fluxer (**beta**) | `ghcr.io/ferdinand99/sylo-fluxer` |
| [`templates/tofarr.xml`](templates/tofarr.xml) | [Tofarr](https://github.com/Ferdinand99/Tofarr) — unofficial companion that builds and updates Tofa collections | `ghcr.io/ferdinand99/tofarr` |

## Install

Search for the app in **Apps** (Community Applications). To use a template
before it shows up there, add this repository under
**Docker → Template repositories**:

```
https://github.com/Ferdinand99/unraid-templates
```

## Support

Open an issue on the app's own repository:
[Sylo](https://github.com/Ferdinand99/Sylo/issues) ·
[Sylo-Fluxer](https://github.com/Ferdinand99/Sylo-Fluxer/issues) ·
[Tofarr](https://github.com/Ferdinand99/Tofarr/issues).

## Maintaining

Each template's `<TemplateURL>` points at its file in this repository, so this
is the copy Unraid refreshes from. Change a template here, not in the app
repositories. `ca_profile.xml` is the repository profile Community Applications
shows under "Ferdinand99's Repository".
