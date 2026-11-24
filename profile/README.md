<div align="center">
  <picture>
    <source
      media="(prefers-color-scheme: dark)"
      srcset="https://raw.githubusercontent.com/engrave-music/.github/main/assets/logo/engrave-music-dark-framed.svg"
    />
    <source
      media="(prefers-color-scheme: light)"
      srcset="https://raw.githubusercontent.com/engrave-music/.github/main/assets/logo/engrave-music-light-framed.svg"
    />
    <img
      alt="engrave-music"
      src="https://raw.githubusercontent.com/engrave-music/.github/main/assets/logo/engrave-music-light-framed.svg"
      width="120"
    />
  </picture>

  <h1>engrave-music</h1>

  <p>Native C++23 music engraving engine and MCP tooling for AI composition.</p>

  <p>
    <strong>English</strong> ·
    <a href="https://github.com/engrave-music/.github/blob/main/profile/README.zh-CN.md">简体中文</a>
  </p>
</div>

## Repositories

| Repository | Description |
| --- | --- |
| [**engrave-mcp**](https://github.com/engrave-music/engrave-mcp) | Native C++ MCP server over stdio JSON-RPC for creating, inspecting, editing, rendering, and exporting musical scores. |
| [**engrave**](https://github.com/engrave-music/engrave) | Headless C++23 music notation, layout, engraving, rendering, and audio synthesis engine (pinned hard fork of MuseScore 5.0 core). |

## Design Principles

- **Native C++23, zero runtime bloat**: Built with Bazel and a hermetic `xclang` toolchain on Windows and Linux — no Node.js, WebAssembly, or desktop MuseScore install at runtime.
- **MuseScore 4.6–5.0 interop**: Agent-authored scores open and remain editable in MuseScore, and MuseScore 4.60–5.00 scores open and remain editable by agents (with native 5.00 export and bounded 4.70 compatibility export).
- **Direct live-memory export**: Export MSCZ/MSCX, MusicXML, MIDI, PDF/SVG/PNG pages, layout positions, and synthesized WAV/FLAC/Opus/MP3 audio directly from the live in-memory document.
- **Open source**: Licensed under **GPL-3.0-only**.
