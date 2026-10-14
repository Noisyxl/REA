<p align="center">
  <img src="rea.png" alt="REA x Opus 5.5" width="100%">
</p>

# REA - Reverse Engineer Anything

🧙 **Point it at any company. Get back the blueprint.**

An AI reverse-engineering framework built on Claude Code and **Opus 5.5**. Give it a product - or an entire company - and Opus takes it apart: every system, every data flow, every decision, with evidence down to the file and function. Then you rebuild it from zero.

## What this is

A structured workflow that turns Opus 5.5 into a full-stack reverse-engineering agent. REA maps everything a company ships - desktop, web, mobile, APIs, smart contracts - traces how each system works end to end, and writes it up as a blueprint you can actually build from.

Built for company-scale targets. A two-person startup or a Microsoft- or Anthropic-sized product surface - hundreds of apps, thousands of endpoints, millions of lines of code - same four commands, same loop. Nothing is guessed: if REA can't prove it from the code, it says so.

⚡ **1** command to start · **4** stages · **0** guesses · **any** stack - Electron, `.exe`, macOS, APK, WASM, EVM, firmware

```
  REA × Opus 5.5                                                               reverse engineer anything
  ──────────────────────────────────────────────────────────────────────────────────────────────────────

  01  /recon <company>      02  /analyze              03  /blueprint            04  /rebuild
      ↓                         ↓                         ↓                         ↓
      map every surface         decompile + read          system map                clean-room spec
      pull artifacts            trace the logic           evidence per claim        your code, from zero
      ↓                         ↓                         ↓                         ↓
      surfaces ready ─────────► behavior mapped ────────► blueprint.md ───────────► verify ──► ship
                                ▲                                                     │
                                └────── diff ≠ original · loop until identical ───────┘
```

## Commands

```
/recon <target>     map every surface a product or company ships, pull the artifacts
/analyze            decompile, read and trace the logic with Opus 5.5
/blueprint          write blueprint.md - systems, flows, evidence, unknowns
/rebuild            clean-room spec -> your own implementation -> verify
```

## Targets

Desktop apps (Electron, `.exe`, macOS) · Websites (structure, scripts, network) · Games (native, Unity, legacy) · Android APKs · Smart contracts (EVM) · .NET, firmware, WASM, Go binaries

---

<sub>MIT · built for research, education, security and interoperability · respect licenses and local law</sub>
