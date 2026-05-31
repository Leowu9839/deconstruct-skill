# 🔍 Deconstruct

> **X-ray vision for AI Skills.**
> 
> *X-Ray Vision for AI Skills.*

---

## Would You Install It Blindly?

Thousands of Skills on GitHub. They all look cool.

But:
- Will it secretly send your data to a third party?
- Does it contain hidden instructions that override your real intent?
- It claims to do A, but actually executes B?
- Are all the permissions it requests truly necessary?

**You can't read the source code of every Skill yourself. But before installing, you should know what it is.**

---

## What This Is

**Deconstruct** is a systematic AI Skill disassembly framework.

Input a complete Skill, output a **structured Markdown disassembly report**. This report serves two readers simultaneously:

- **Humans**: Hierarchical document with TOC, jump to sections as needed
- **AI**: Structured context supplement, helping understand design intent, boundaries, and vulnerabilities

### Core Capabilities

| Capability | Description |
|------------|-------------|
| 🔬 **Technical Anatomy** | Uncover what techniques the Skill uses — external APIs, MCP, tool calls, knowledge bases, chaining, persistence |
| 🔐 **Security Audit** | Data flow, external call necessity, hidden instructions, permission boundaries, intent consistency — each with ✅/⚠️/❌ and plain-language conclusions |
| 🧩 **Cognitive Component Extraction** | Abstract design decisions into reusable components, each with essence, applicable conditions, variants, synergies |
| 🧨 **Vulnerability Analysis** | Observational + stress-tested, actively finding the most critical weak points |
| 🚀 **Evolution Directions** | Plugin enhancements, chaining directions, rebuild trade-offs — know where to start cutting |

### Security Audit Five Checks

```
Data Flow        → Will your content flow to third parties?
External Call Necessity → Does every request have business justification?
Hidden Instructions → Any role hijacking or intent-overriding statements?
Permission Boundaries → Do requested permissions match functionality?
Intent Consistency → Does claimed purpose match actual execution?
```

> **Every audit conclusion has two parts: technical judgment + plain-language explanation ("What this means for you").**
> 
> Non-technical users will know "Can I use this Skill?" after reading.

---

## Real Example

**Input**: Complete implementation of a "Smart Writing Assistant" Skill

**Deconstruct Output**:

```markdown
## 📋 Overview
> This is a tool that turns long articles into bullet-point summaries. Safe to use. Doesn't send your content to anyone.

## 🔬 Technical Anatomy
| Layer | Content | Plain Language |
|-------|---------|----------------|
| External API | None | No internet connection |
| MCP Calls | None | No external tools called |
| Tool Calls | Code execution (Python) | Runs text tokenization and statistics |
| Knowledge Source | Pure model built-in | AI's own remembered grammar rules |
| Chaining | Single-step generation | One-shot output |
| Persistence | None | No records saved |

## 🔐 Security Audit
| Audit Item | Status | What This Means For You |
|------------|:------:|-------------------------|
| Data Flow | ✅ | Your input is only processed in this conversation, not sent to any third party |
| External Calls | ✅ | No internet needed, no API leakage worries |
| Hidden Instructions | ✅ | No statements overriding your intent found |
| Permission Boundaries | ✅ | Only requests text processing permissions, reasonable |
| Intent Consistency | ✅ | Claims writing assistance, actually provides writing assistance |

## 🧩 Cognitive Components
- **Component: Segmented Summarization** — Split long text into chunks, summarize each, then merge
- **Component: Keyword Anchoring** — Use TF-IDF to find high-frequency words, ensure summary stays on track

## 🧨 Vulnerabilities
- When input exceeds 5,000 words, segmentation boundaries may cut semantic meaning
- When switching to non-Chinese languages, keyword extraction accuracy drops

## 🚀 Evolution Directions
- Pre-chain: Content scraping Skill (responsible for extracting text from web/docs)
- Post-chain: Layout beautification Skill (responsible for turning summary into PPT/poster)
```

**Value**: Read the report in 5 minutes. Know if this Skill is safe, worth learning from, and how to improve it.

---

## Who Is It For

| User | Scenario |
|------|----------|
| 🔍 Skill Learners | See a cool Skill, want to disassemble and learn its thinking |
| 🛡️ Security-Cautious Users | Found a Skill on GitHub, audit before use |
| 🔧 Skill Improvers | Want to modify a Skill, know where to start cutting |
| 🧬 Skill Combiners | Want to merge two Skills, reports make finding combinations easy |
| 🏗️ Skill Creators | More components accumulated = lower assembly cost |

---

## Quick Start

```markdown
(Paste the complete Skill content)

"Deconstruct it"
"Break this Skill down for me"
"What was the thinking behind this Skill"
"Give me a disassembly analysis"
```

**Any of the above expressions automatically triggers disassembly.**

---

## Design Philosophy

### Innovation 1: Non-Technical Users First

Technical users can read the original document. The people who really need this report are those who can't understand the original implementation.

- Technical terms must include plain-language explanations on first appearance
- Every security audit conclusion must explain "What this means for you"
- The overview must contain a one-sentence summary anyone can understand

### Innovation 2: Dual-Purpose Reports

The same Markdown report:
- **Humans read**: Hierarchical document with TOC
- **AI reads**: Structured context supplement. Give AI the original Skill, it only knows "what to do"; give AI Skill + disassembly report, it also knows "why it's done this way, where the boundaries are, what can go wrong"

### Innovation 3: Reports as Infrastructure

Throw a batch of disassembly reports at AI and ask "Can these be combined?" — component lists are standardized, vulnerabilities listed, evolution clues present — **the report compresses a Skill into an "interface document."**

The more you accumulate, the easier combination and evolution become. Compound interest effect.

### Innovation 4: Learning and Security Audit Unified

The process of learning IS the process of auditing. The discoveries from auditing ARE the learning content. **Two birds, one stone.**

---

## File Structure

```
deconstruct-skill/
├── README.md        # This file (Chinese)
├── README_EN.md     # English version
├── Skill.md         # Complete disassembly framework & execution specs
└── Skill_v1.1       # Updated version notes
```

---

## ⚠️ Boundaries & Limitations

- **Input Threshold**: Must be complete implementation, no reverse inference
- **Security Audit Depth**: Text-based static analysis, cannot detect actual runtime network behavior
- **Linkage Fields**: Current version synergy relationships based on components within this disassembly
- **Disassembly Depth**: Positively correlated with input complexity — simple Skills naturally produce thinner reports

---

## Author

**Leo Wu** · [GitHub](https://github.com/Leowu9839)

## License

MIT
