# blendOS Tracks

* GNOME: `gnome`
* Plasma: `plasma`
* Cinnamon: `cinnamon`
* COSMIC: `cosmic`
* LXQT: `lxqt`
* MATE: `mate`
* XFCE: `xfce`

## Forking

You can fork this to use it as a base for your own tracks, but be aware that the Github and Codeberg mirrors are read-only (and have pull requests disabled). If you want to propose your changes to this repo, use [the Gitlab](https://git.blendos.co/blendos/tracks).

## Example GNOME `/system.yaml` (vanilla)

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/blend-os/tracks/raw/main'

track: 'gnome'
```

## Example GNOME `/system.yaml` with Caddy

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/blend-os/tracks/raw/main'

track: 'gnome'

packages:
    - 'micro'
    - 'caddy'

services:
    - 'caddy'

package-repos:
    - name: 'chaotic-aur'
      repo-url: 'https://cdn-mirror.chaotic.cx/$repo/$arch'
```