# Ferdinand99's Unraid templates

Unraid Docker templates for [Community Applications](https://ca.unraid.net).
This repository only holds the templates; each app lives in its own
repository.

| Template | App | Image |
| --- | --- | --- |
| [`templates/keen-kestrel.xml`](templates/keen-kestrel.xml) | [Keen Kestrel](https://github.com/Ferdinand99/Keen-Kestrel) — self-hosted, Sentry-compatible error tracking and cookieless analytics | `ghcr.io/ferdinand99/keen-kestrel` |
| [`templates/sylo.xml`](templates/sylo.xml) | [Sylo](https://github.com/Ferdinand99/Sylo) — multi-function bot for Discord and Fluxer with a web dashboard | `docker.io/iwgamin/sylo` |
| [`templates/tofarr.xml`](templates/tofarr.xml) | [Tofarr](https://github.com/Ferdinand99/Tofarr) — unofficial companion that builds and updates Tofa collections | `ghcr.io/ferdinand99/tofarr` |
| [`templates/wise-wren.xml`](templates/wise-wren.xml) | [Wise Wren](https://github.com/Ferdinand99/Wise-Wren) — keeps your Docker containers up to date, with snapshots, health checks and rollback (the server) | `ghcr.io/ferdinand99/wise-wren` |
| [`templates/wise-wren-agent.xml`](templates/wise-wren-agent.xml) | Wise Wren Agent — runs on each server Wren updates; gets the Docker socket, so it is root-equivalent | `ghcr.io/ferdinand99/wise-wren-agent` |
| [`templates/vigilant-vole.xml`](templates/vigilant-vole.xml) | [Vigilant Vole](https://github.com/Ferdinand99/Vigilant-Vole) — lightweight uptime monitor with status pages, an Uptime Kuma alternative | `ghcr.io/ferdinand99/vigilant-vole` |

## Install

Search for the app in **Apps** (Community Applications). To use a template
before it shows up there, add this repository under
**Docker → Template repositories**:

```
https://github.com/Ferdinand99/unraid-templates
```

## Support

Open an issue on the app's own repository:
[Keen Kestrel](https://github.com/Ferdinand99/Keen-Kestrel/issues) ·
[Sylo](https://github.com/Ferdinand99/Sylo/issues) ·
[Tofarr](https://github.com/Ferdinand99/Tofarr/issues) ·
[Vigilant Vole](https://github.com/Ferdinand99/Vigilant-Vole/issues) ·
[Wise Wren](https://github.com/Ferdinand99/Wise-Wren/issues).

## Sylo-Fluxer

The separate Sylo-Fluxer fork and its template are gone: [Sylo](https://github.com/Ferdinand99/Sylo)
4.0 runs on Fluxer itself. Install the **Sylo** template and fill in the `FLUXER_*` settings, with or
without the Discord ones. The old fork is archived, and its data does not carry over; see
[Coming from Sylo-Fluxer](https://github.com/Ferdinand99/Sylo/blob/main/docs/fluxer.md#coming-from-sylo-fluxer).

## Maintaining

Each template's `<TemplateURL>` points at its file in this repository, so this
is the copy Unraid refreshes from. Change a template here, not in the app
repositories. `ca_profile.xml` is the repository profile Community Applications
shows under "Ferdinand99's Repository".
