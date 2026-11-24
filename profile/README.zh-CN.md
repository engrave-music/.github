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

  <p>面向 AI 作曲的原生 C++23 制谱引擎与 MCP 工具链。</p>

  <p>
    <a href="https://github.com/engrave-music">English</a> ·
    <strong>简体中文</strong>
  </p>
</div>

## 仓库列表

| 仓库 | 说明 |
| --- | --- |
| [**engrave-mcp**](https://github.com/engrave-music/engrave-mcp/blob/main/README.zh-CN.md) | 原生 C++ MCP 服务，通过 stdio JSON-RPC 创建、查询、编辑、排版并导出乐谱。 |
| [**engrave**](https://github.com/engrave-music/engrave/blob/main/README.zh-CN.md) | 无头 C++23 记谱、排版、制谱、渲染与音频合成引擎（MuseScore 5.0 核心的固定硬分叉）。 |

## 设计原则

- **原生 C++23，零冗余运行时**：基于 Bazel 与隔离的 `xclang` 工具链支持 Windows 与 Linux，运行时无需 Node.js、WebAssembly 或桌面版 MuseScore。
- **MuseScore 4.6–5.0 互操作**：Agent 生成的乐谱可在 MuseScore 中打开并继续编辑，MuseScore 4.60–5.00 乐谱也可由 Agent 打开编辑（默认导出 5.00，并提供有界 4.70 兼容导出）。
- **内存实时直出**：直接从内存中的实时文档导出 MSCZ/MSCX、MusicXML、MIDI、PDF/SVG/PNG 页面、排版位置数据以及 WAV/FLAC/Opus/MP3 合成音频。
- **开源许可**：采用 **GPL-3.0-only** 许可证。
