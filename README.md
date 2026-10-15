# Awesome-AI-Reverse-Engineering

# Top AI Reverse Engineering Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Agent-Assisted Binary Analysis, Decompilation & Software Reconstruction*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Reverse Engineering**. These tools enable developers and security researchers to investigate compiled software without source code—tracing application behavior down to native binaries, recovering pseudocode from stripped executables, and reconstructing equivalent functionality through agent-driven analysis.

**Examples** include IDA Pro, Hex-Rays, Binary Ninja, Ghidra, JEB Decompiler, Hopper, Radare2, Cutter, Veles, and Angr (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, agent-driven binary analysis, and open decompilation pipelines—ideal for security researchers, developers, and reverse engineers seeking transparent, vendor-independent analysis tools.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[IDA Pro](https://hex-rays.com/ida-pro/)**  
  Industry-standard disassembler and debugger with the Hex-Rays decompiler. The most mature and feature-complete commercial reverse engineering platform, with extensive plugin ecosystem and scripting support.

- **[Hex-Rays](https://hex-rays.com/)**  
  The decompiler engine powering IDA Pro. Converts assembly to high-level pseudocode across multiple architectures. **The reference implementation for commercial decompilation.**

- **[Binary Ninja](https://binary.ninja/)**  
  Modern reverse engineering platform with a clean API, multi-architecture support, and collaborative features. **The most developer-friendly commercial RE tool.**

- **[JEB Decompiler](https://www.pnfsoftware.com/)**  
  Commercial decompiler for Android, ARM, and other platforms. **The standard for Android APK analysis.**

- **[Hopper](https://www.hopperapp.com/)**  
  macOS/Linux disassembler and decompiler with a native interface. **The most polished macOS-native RE tool.**

## Open-Source GitHub Projects

- **[Ghidra](https://github.com/NationalSecurityAgency/ghidra)**  
  **The NSA's open-source software reverse engineering suite** (Apache-2.0). **50,000+ GitHub stars.** Decompiler, disassembler, debugger, and scripting support across multiple architectures. **The reference open-source RE platform** and the engine behind most agent-driven analysis tools.

- **[REA (Reverse Engineer Anything)](https://github.com/morluto/rea)**  
  **The most rapidly adopted open-source AI reverse engineering agent platform** (MIT). **120,000+ GitHub stars within days of launch**—one of the fastest-growing repositories of 2026 . **The MCP server that connects AI agents to Ghidra, Hopper, IDA, and other analysis engines** . **Analyzes native binaries** (Mach-O, ELF, PE), **JavaScript/Electron apps**, **.NET assemblies**, **Android APKs**, **firmware**, **websites**, and **saved network captures** . **Returns structured evidence**—decompiled code, call graphs, application graphs—for agents to explain or build from . **Local analysis**—targets never upload . **Powers agent-driven workflows** in Claude Code, Codex, Cursor, Gemini CLI, and Hermes . **The emerging standard for AI-assisted reverse engineering.**

- **[Cutter](https://github.com/rizinorg/cutter)**  
  **Free and open-source reverse engineering platform** (GPL-3.0) powered by Rizin (Radare2 fork). **GUI for disassembly and decompilation** with Ghidra decompiler integration. **The most user-friendly open-source RE interface.**

- **[Radare2](https://github.com/radareorg/radare2)**  
  **Advanced open-source reverse engineering framework** (LGPL-3.0). **20,000+ GitHub stars.** Command-line driven with extensive scripting support. **The foundation for Cutter** and many other RE tools.

- **[Angr](https://github.com/angr/angr)**  
  **Platform-agnostic binary analysis framework** (BSD-2-Clause) from UC Santa Barbara. **8,000+ GitHub stars.** **Symbolic execution**, **concolic execution**, and **control-flow analysis**. **The standard open-source tool for automated vulnerability discovery.**

- **[Veles](https://github.com/vuku/veles)**  
  Open-source binary analysis tool (Apache-2.0) for data visualization and pattern discovery. **The most focused open-source tool for binary pattern analysis.**

- **[CutterMCP+](https://pypi.org/project/iflow-mcp_restkhz-CutterMCP-plus/)**  
  **MCP server for Cutter** (open-source). **Automated reverse engineering via LLMs**—provides `list_functions`, `decompile`, `disasm_text`, `xrefs_to`, `rename_function`, and other tools for AI agents . **Demonstrated solving HackTheBox CTF challenges autonomously**—anti-analysis techniques, VM analysis, and malware triage without human intervention .

- **[Reversecore MCP](https://pypi.org/project/reversecore-mcp/)**  
  **Security-first MCP server for reverse engineering and malware analysis** (open-source, 203 GitHub stars) . **Structured access to Radare2, r2ghidra, YARA, LIEF, Capstone, angr, Qiling, Volatility3, and Scapy** . **Explicit workspace boundaries, input validation, non-root containers, and security regression testing** . **Static analysis, malware triage, symbolic execution, forensics, and SAST** in one server .

- **[OGhidra](https://github.com/LLNL/OGhidra)**  
  **AI-driven binary analysis tool from Lawrence Livermore National Laboratory** (BSD-3-Clause) . **Uses locally hosted agentic AI to automatically reverse engineer binaries** for malware and vulnerabilities . **RAG-powered semantic search** over analyzed functions—find similar functions by intent, not just name . **Session management** preserves analysis across sessions .

- **[Open-ReverseLab](https://github.com/LING71671/open-reverselab)**  
  **Open-source AI reverse-engineering agent platform and MCP server** for Ghidra, Frida, x64dbg, and Rizin . **100+ MCP tools** and a **194-article runnable knowledge base** . **Automated PE/APK/binary analysis, CTF, and malware research** . **Modular board system**—install only the tools you need .

- **[Kong](https://pypi.org/project/kong-re/)**  
  **The Agentic Reverse Engineer** (open-source). **Fully autonomous pipeline**—runs complete analysis with no manual intervention . **Call-graph-ordered analysis**—leaf functions named first, so callers benefit from resolved context . **Agentic deobfuscation**—identifies and removes control flow flattening, bogus control flow, string encryption, and VM protection . **Semantic synthesis**—unifies naming conventions and synthesizes struct definitions across the entire binary . **Cost-tracking** for LLM calls .

- **[AIDebug](https://pypi.org/project/1200km-aidebug/)**  
  **AI-assisted malware reverse-engineering debugger** (open-source) . **Turns function behavior into ATT&CK mappings, YARA rules, IOC exports, and analyst reports** . **Static analysis** (PE/ELF parsing, Capstone disassembly, pattern detection) and **dynamic mode** (Frida instrumentation) . **Safe examples** included—no live malware in the repository .

### Additional Strong Open-Source Options

- **[Rizin](https://github.com/rizinorg/rizin)** — Open-source RE framework (LGPL-3.0), fork of Radare2. **The engine behind Cutter** .
- **[GhidraMCP](https://github.com/LaurieWired/GhidraMCP)** — MCP server for Ghidra (Apache-2.0). **The original MCP bridge** for Ghidra-based agent workflows.
- **[Qiling](https://github.com/qilingframework/qiling)** — Advanced binary emulation framework (Apache-2.0). **Cross-platform emulation** for Windows, Linux, macOS, Android, and IoT firmware.
- **[Frida](https://github.com/frida/frida)** — Dynamic instrumentation toolkit (wxWindows Library Licence). **The standard for runtime binary analysis.**
- **[LIEF](https://github.com/lief-project/LIEF)** — Library to parse and modify executable formats (Apache-2.0).
- **[Capstone](https://github.com/capstone-engine/capstone)** — Disassembly framework (BSD-3-Clause). **The most widely used disassembly engine.**
- **[YARA](https://github.com/VirusTotal/yara)** — Pattern matching for malware identification (Apache-2.0).
- Community **n8n** workflows for reverse engineering alerting and analysis pipeline automation.

**Frameworks for building custom systems**: Combine **REA** for agent-driven analysis orchestration with **Ghidra** for decompilation, **CutterMCP+** or **Reversecore MCP** for tool integration, **Angr** for symbolic execution, and **Kong** for autonomous deobfuscation—creating a fully self-hosted, enterprise-grade reverse engineering platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- **Reverse engineering tools are for lawful research, education, interoperability, software preservation, and analysis of software you own or are authorized to examine.** Unauthorized reverse engineering may violate copyright law, end-user license agreements, and the DMCA. **Always obtain proper authorization before analyzing third-party software.**
- **REA's explosive growth signals a paradigm shift.** 120,000+ stars in days . Replit CEO Ahmad Msad: "AI-driven reverse engineering and decompilation is incredible. Soon, all software may effectively become open source" . **The "closed-source moat" is being eroded by AI agents that can read binaries.**
- **But REA doesn't outperform a competent agent with the right tools.** Korben's independent testing: "REA doesn't do any better than a Claude you ask to install Ghidra and use it" . **REA's value is convenience and standardization, not superhuman capability.**
- **Agent-driven analysis has real limitations.** Korben's test showed the agent "was searching for these codes by name before having seen them"—the model already knew Wolfenstein 3D's cheat codes . **Attribution of discovery is difficult when models have memorized training data.**
- **Security and ethics matter.** Reversecore MCP is "security-first" with explicit workspace boundaries, input validation, and non-root containers . **Run untrusted binaries only in isolated VMs or hardened containers** .
- **Commercial tools retain their licenses.** REA grants no license for IDA Pro, Hopper, or JEB . **Cracked copies and unauthorized key sharing are explicitly prohibited.**
- Self-hosted open-source solutions require proper security hardening, analysis engine configuration, and ongoing maintenance. **Reverse engineering infrastructure is security-critical—compromised analysis tools can inject malicious output.**

---

**Made for security researchers, reverse engineers, and developers building transparent binary analysis solutions.**  
Let's make AI Reverse Engineering more open, data-driven, and accountable.
