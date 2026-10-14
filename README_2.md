<p align="center">
  <img src="rea-banner.png" alt="REA — Reverse Engineer Anything" width="100%">
</p>

<p align="center">
  <b>Point it at any product. Get back the blueprint.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-0d1117?style=flat-square&labelColor=0d1117&color=2f81f7" alt="MIT">
  <img src="https://img.shields.io/badge/agent-Opus%205.5-0d1117?style=flat-square&labelColor=0d1117&color=2f81f7" alt="Opus 5.5">
  <img src="https://img.shields.io/badge/works%20with-Codex%20%C2%B7%20Cursor-0d1117?style=flat-square&labelColor=0d1117&color=30363d" alt="Codex, Cursor">
</p>

<br>

Pick a company. REA takes apart everything it ships — desktop app, web app, mobile app, APIs, smart contracts — and hands you the blueprint: every system, every data flow, every decision, with evidence down to the file and function.

Then you rebuild it. From zero.

<br>

```
$ rea analyze --target "any company"

  surfaces    web · desktop · android · api · contracts
  traced      every call, every request, every state change
  mapped      auth · billing · sync · search · storage · ...
  output      blueprint.md  — how it works, with evidence

$ rea rebuild --from blueprint.md
```

<br>

## How it works

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'ui-monospace, SFMono-Regular, Menlo, monospace','fontSize':'13px','primaryColor':'#0d1117','primaryTextColor':'#e6edf3','primaryBorderColor':'#30363d','lineColor':'#2f81f7','clusterBkg':'#010409','clusterBorder':'#2f81f7','titleColor':'#2f81f7','edgeLabelBackground':'#0d1117','tertiaryColor':'#0d1117'}}}%%
flowchart LR
  T(["target<br/>any company · app · binary"])

  subgraph S1["01 · recon"]
    direction TB
    a1["surface map<br/>apps · sites · APIs"] --> a2["pull artifacts<br/>bundles · APKs · bytecode"]
  end

  subgraph S2["02 · analyze"]
    direction TB
    b1["decompile + read"] --> b2["trace logic<br/>calls · state · network"]
  end

  subgraph S3["03 · blueprint"]
    direction TB
    c1["system map<br/>services · data · auth"] --> c2["evidence<br/>file · function · line"]
  end

  subgraph S4["04 · rebuild"]
    direction TB
    d1["clean-room spec"] --> d2["your code<br/>from zero"]
  end

  V{"same<br/>behavior?"}
  OK(["ship"])

  T --> S1 --> S2 --> S3 --> S4 --> V
  V -- "no · diff" --> S2
  V -- "yes" --> OK
```

<br>

## Targets

| Target | What REA reads |
|---|---|
| Desktop apps | Electron, `.exe`, macOS apps — Notion, Slack, Discord |
| Websites | page structure, scripts, network requests |
| Games | native binaries, Unity, legacy titles |
| Android | decompiled APKs, permissions, logic |
| Smart contracts | EVM bytecode, functions, risks |
| Everything else | .NET, firmware, WASM, Go binaries |

<br>

## Why

Understand how anything works. Get exact files, functions and logic — not guesses. Learn, audit, and build your own version.

<br>

---

<p align="center">
  <sub>MIT · for research, education, security and interoperability · respect licenses and local law</sub>
</p>
