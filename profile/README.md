# 界外共行 · Jiewaigongxing

> DNA-First full-stack code generation. Tell AI editors what you want — get a real Spring Boot backend, Vue3 admin panel, UniApp mobile app, and marketing website. All generated, all consistent, all driven by declarative **XDNA** definitions.

[![Website](https://img.shields.io/badge/Website-jiewaigongxing.com-2563EB)](https://jiewaigongxing.com)
[![License](https://img.shields.io/badge/Public_skill-Apache--2.0-green)](https://github.com/jiewaigongxing/jiey_skill/blob/main/LICENSE)
[![npm](https://img.shields.io/npm/v/jieymcp?label=jieymcp)](https://www.npmjs.com/package/jieymcp)

---

## What we do

We build the **AI-native full-stack code generation platform** for teams who want production-grade systems — not toy demos — from a single requirements conversation.

```
Idea  →  XDNA (declarative domain)  →  jieymcp engine  →  shipped product
                                          │
                          Java backend ───┤
                          Vue admin    ───┤
                          UniApp mobile──┤
                          Website      ───┘
```

The core idea: **API is a projection of Action.** You declare entities + actions in XDNA; controllers, request bodies, state machines, ownership checks, side effects, and events are all derived by the compiler. You never write controllers by hand. Your AI editor follows the methodology and uses our MCP engine to generate the artefacts.

## Open-source projects

| Project | What it is |
|---------|-----------|
| **[jiey_skill](https://github.com/jiewaigongxing/jiey_skill)** | DNA-First methodology skill for Cursor / Claude Code / OpenCode. Gives the AI editor the workflow + hard rules; engine details are fetched at runtime via MCP. Apache-2.0. |
| **[jieymcp-cursor-plugin](https://github.com/jiewaigongxing/jieymcp-cursor-plugin)** _(coming soon)_ | One-click Cursor plugin that wires the methodology + MCP server. |

## Commercial products

| Product | What it is |
|---------|-----------|
| **`jieymcp` (npm)** | Local MCP server + codegen engine. Java + Vue + UniApp + website from XDNA. Login required (`jieymcp login`). [npm](https://www.npmjs.com/package/jieymcp) |
| **Jiey Studio** _(closed-source)_ | Desktop IDE on top of `jieymcp`. macOS / Windows / Linux. |

## Quick start

```bash
# 1. Install the engine
npm install -g jieymcp

# 2. Login (required — opens browser)
jieymcp login

# 3. In Cursor / Claude Code, install the methodology skill
#    Cursor: install plugin / clone https://github.com/jiewaigongxing/jiey_skill
#    Claude Code: claude --skill /path/to/jiey_skill/SKILL.md

# 4. Ask the AI to build something
#    e.g. "用 jieymcp 帮我做一个连锁奶茶店管理系统"
```

The AI editor reads our open methodology, calls `trigger_codegen` on the local MCP server, and the engine writes a full project. Detailed schemas / patterns / conventions are returned at runtime via `jiey_skill_doc(slice="...")` — they live inside the engine, not in the open-source repo.

## Why the split

| Open source | Proprietary |
|-------------|-------------|
| Methodology, philosophy, 5-phase workflow, hard rules | Codegen engine (Spring Boot / Vue3 / UniApp templates) |
| Cursor / Claude / OpenCode plugin shells | Compiler, runtime Action Pipeline, Saga, state-machine wiring |
| Public DNA examples | Industry knowledge base, plugin marketplace, license, telemetry |

The methodology is the **playbook**; the engine is the **production line**. We open the playbook so AI editors can drive the engine reliably; we keep the engine proprietary because that's where the real moat lives.

## Get involved

- **Try it:** [jiewaigongxing.com](https://jiewaigongxing.com)
- **Read the methodology:** [jiey_skill](https://github.com/jiewaigongxing/jiey_skill)
- **Architect tier (industry packs + revenue share):** [Architect program](https://jiewaigongxing.com/developers)
- **Contact:** dev@jiewaigongxing.com

---

<sub>© Jiewaigongxing. The methodology is Apache-2.0; the engine, Studio, and platform service are proprietary.</sub>
