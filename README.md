# at-spi2-core

xlings payload repacked from upstream binaries (conda-forge / Debian) by
[`.agents/tools/repack/repack.py`](https://github.com/openxlings/xim-pkgindex/tree/main/.agents/tools/repack).
Recipe: [`xim-pkgindex`](https://github.com/openxlings/xim-pkgindex) `pkgs/a/at-spi2-core.lua`.

Every release asset carries `PROVENANCE.md` (upstream artefacts, sha256, the exact command) and a `.sha256` sidecar.

## Sources

| artefact | sha256 | origin |
|---|---|---|
| https://conda.anaconda.org/conda-forge/linux-64/at-spi2-core-2.40.3-h0630a04_0.tar.bz2 | `c4f9b66bd94c40d8f1ce1fad2d8b46534bdefda0c86e3337b28f6c25779f258d` | conda-forge at-spi2-core 2.40.3 h0630a04_0 (LGPL-2.1-or-later) |

## Command

```
.agents/tools/repack/repack.py \
    --name at-spi2-core \
    --version 2.40.3 \
    --arch x86_64 \
    --src https://conda.anaconda.org/conda-forge/linux-64/at-spi2-core-2.40.3-h0630a04_0.tar.bz2#c4f9b66bd94c40d8f1ce1fad2d8b46534bdefda0c86e3337b28f6c25779f258d \
    --drop 'share/dbus-1/*' \
    --drop 'share/defaults/*' \
    --require lib/libatspi.so.0
```

