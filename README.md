# argolex.dev.download

Download host for **Argolex**. This repository exists only to serve release
assets over HTTPS — it is a distribution endpoint, not source code.

**You never need to clone this repository.** The Argolex installer and the
in-app updater fetch what they need directly from the release assets below.

## Release layout

### `models-<sha12>` — model archives (pre-release)

One release per model set, carrying a single asset:

```
argolex-models-<sha12>.7z
```

`<sha12>` is the first 12 hex characters of the SHA-256 of the app's
`models_manifest.json`, so the archive name pins the exact model set the build
expects. The archive contains exactly the files the manifest lists, at their
manifest-relative paths; extracting it into `Argolex_Data/StreamingAssets/models`
reproduces the desktop build's model layout.

The itch.io and Gumroad installers download this archive during setup and verify
it against the SHA-256 recorded in [`models.json`](models.json).

These releases are marked **pre-release** and are never marked "latest".

### `v<version>` — app releases

The installers and `latest.json` (the update feed). `releases/latest` always
resolves to an app release, never to a model archive, so the updater can rely on
it.

## `models.json`

The current model archive: tag, asset name, download URL, byte size, SHA-256,
the manifest SHA-256 it was built from, the file count and the total
uncompressed size. Installers read this to know what to fetch and what to verify.

## `LICENSES/`

Licence texts for the model families carried in the archive, one folder per
top-level directory in the manifest:

| folder | model family | licence |
| --- | --- | --- |
| `LICENSES/kokoro` | Kokoro-82M | Apache 2.0 |
| `LICENSES/qwen3.5-gguf` | Qwen3.5 | Apache 2.0 |
| `LICENSES/moonshine` | Moonshine | MIT |
| `LICENSES/silero-vad` | Silero VAD | MIT |

Each folder holds the licence text and a `SOURCE.md` naming the upstream page.

## No model files in git

**Model weights are never committed to this repository.** No `.onnx`, `.gguf`,
`.bin`, `.safetensors` or `.7z` file is tracked here. Models exist only as
release assets. The git tree holds nothing but this README, `models.json`,
the licence texts and `.gitattributes`.
