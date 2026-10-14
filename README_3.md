<p align="center">
  <img src="rea.png" alt="REA" width="280">
</p>

# REA — Reverse Engineer Anything

An AI reverse-engineering framework built on Claude Code and **Opus 5.5**. Point it at any product, let Opus take it apart, and get back the blueprint: every system, every data flow, every decision — with evidence down to the file and function. Then rebuild it from zero.

## What this is

A structured workflow that turns Opus 5.5 into a full-stack reverse-engineering agent. Give it one app — or an entire company. REA maps everything that company ships (desktop, web, mobile, APIs, smart contracts), traces how each system works end to end, and writes it up as a blueprint you can actually build from.

The core pipeline — recon, analysis, blueprint, clean-room rebuild — is **target- and stack-agnostic**. Electron, `.exe`, macOS apps, APKs, WASM, EVM bytecode, firmware: same four commands, same loop. Nothing is guessed. If REA can't prove it from the code, it says so.

```
  REA  ::  reverse engineer anything  ::  agent: Opus 5.5
  ──────────────────────────────────────────────────────────────────────────────────────

  /recon <company>      /analyze               /blueprint             /rebuild
    │                     │                      │                      │
    ▼                     ▼                      ▼                      ▼
  Map every surface     Opus 5.5 reads         System map             Clean-room spec
  web · desktop ·       every bundle,          auth · billing ·       from blueprint
  mobile · APIs         binary and APK         sync · storage
    │                     │                      │                      │
    ▼                     ▼                      ▼                      ▼
  Pull artifacts        Trace the logic        Evidence for           Opus writes your
  bundles · APKs ·      calls · state ·        every claim            version, from zero
  bytecode · WASM       network · auth         file · fn · line
    │                     │                      │                      │
    ▼                     ▼                      ▼                      ▼
  Surfaces ready        Behavior mapped        blueprint.md           Reviewer agent diffs
  -> /analyze           -> /blueprint          -> /rebuild            behavior -> ship
                                                                        │
                          ▲                                             │
                          └── diff ≠ original · loop until identical ───┘
```

## Commands

```
/recon <target>     map every surface a product or company ships, pull the artifacts
/analyze            decompile, read and trace the logic with Opus 5.5
/blueprint          write blueprint.md — systems, flows, evidence, unknowns
/rebuild            clean-room spec -> your own implementation -> verify
```

## Targets

Desktop apps (Electron, `.exe`, macOS) · Websites (structure, scripts, network) · Games (native, Unity, legacy) · Android APKs · Smart contracts (EVM) · .NET, firmware, WASM, Go binaries

---

<sub>MIT · built for research, education, security and interoperability · respect licenses and local law</sub>
