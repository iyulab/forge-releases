# forge-releases (Deprecated 2026-04-27)

This repo previously hosted GitHub Releases for all 6 Forge apps via per-channel `latest-{app}.yml` metadata files. The shared-repo strategy proved incompatible with electron-updater's `GitHubProvider` ("repo-level latest" assumption), causing cross-channel 404s when other apps released later.

**Migrated to per-app release repos (2026-04-27):**

| App | Repo |
|---|---|
| Forge-Lens | [iyulab/forge-releases-lens](https://github.com/iyulab/forge-releases-lens) |
| Forge-SPC | [iyulab/forge-releases-spc](https://github.com/iyulab/forge-releases-spc) |
| Forge-FMEA | [iyulab/forge-releases-fmea](https://github.com/iyulab/forge-releases-fmea) |
| Forge-8D | [iyulab/forge-releases-8d](https://github.com/iyulab/forge-releases-8d) |
| Forge-SOP | [iyulab/forge-releases-sop](https://github.com/iyulab/forge-releases-sop) |
| Forge-DOE | [iyulab/forge-releases-doe](https://github.com/iyulab/forge-releases-doe) |

Existing releases (lens-v0.7.7 etc.) remain available here for installed users whose auto-update endpoint still points to this repo. New releases (v0.7.8+) are published in the per-app repos. Installers from those new releases auto-redirect to their respective repo for subsequent updates.

App downloads: https://forge-tools.work
