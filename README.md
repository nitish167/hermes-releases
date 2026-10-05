# hermes-releases

Release hosting for the Hermes desktop app — this repository holds **Releases** (the macOS payload asset) and the **GitHub Pages site** (installers, manifest, key). There is no source code here.

## Install

Standard (installs to ~/Applications on an Intel Mac, macOS 12 or newer):

```
curl -fsSL https://nitish167.github.io/hermes-releases/install | bash
```

Portable (runs from a USB stick, writes nothing to the host):

```
curl -fsSL https://nitish167.github.io/hermes-releases/install-portable | bash
```

The installer downloads the payload from this repository Releases, verifies its SHA-256, writes the NVIDIA key, relocalises the engine and runs an 11-check health gate. **Do not download the release asset manually** — it is an archive for the installer, not a runnable app.

Site files live on the `pages` branch, served at https://nitish167.github.io/hermes-releases/