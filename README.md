# hermes-releases

Release hosting for the Hermes desktop app — this repository holds **Releases only** (the macOS payload asset). There is no source code here.

## Install

Standard (installs to ~/Applications on an Intel Mac, macOS 12 or newer):

```
curl -fsSL https://agent-167.web.app/install | bash
```

Portable (runs from a USB stick, writes nothing to the host):

```
curl -fsSL https://agent-167.web.app/install-portable | bash
```

The installer downloads the payload from this repository's Releases, verifies its SHA-256, writes the NVIDIA key, relocalises the engine and runs an 11-check health gate. **Do not download the release asset manually** — it is an archive for the installer, not a runnable app.
