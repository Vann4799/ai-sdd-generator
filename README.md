# ⚙️ AI SDD Generator

Generate comprehensive **Software Design Documents** through warm, conversational AI interviews.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-0.2.0-blue.svg)]()

> Inspired by advanced prompting techniques from Claude Fable 5, Cursor, Lovable, and Devin.

## ✨ Features

- 🗣️ **Conversational Interview** — AI asks questions one by one, like talking to a friend
- 🇮🇩 **Indonesian & English** — Natural bilingual support
- 🎯 **Fable 5 Style** — Warm, friendly, no AI-isms
- 📝 **Non-Technical Summary** — Simple explanation at the end
- 🔧 **Multi-Tool** — Works with Claude Code, Codex, OpenCode, Hermes Agent

## 📦 Installation

### Claude Code
```bash
git clone https://github.com/Vann4799/ai-sdd-generator.git ~/.claude/ai-sdd-generator
```

### Codex
```bash
git clone https://github.com/Vann4799/ai-sdd-generator.git ~/.codex/ai-sdd-generator
```

### OpenCode
```bash
git clone https://github.com/Vann4799/ai-sdd-generator.git ~/.opencode/skills/ai-sdd-generator
```

### Hermes Agent
```bash
hermes skills install Vann4799/ai-sdd-generator
```

## 🎯 Usage

Simply say:

```
"Buat SDD untuk aplikasi kasir toko"
```

## 📋 Interview Questions

| # | Question (ID) | Question (EN) |
|---|--------------|---------------|
| 1 | Apa nama aplikasinya? | What's the project name? |
| 2 | Jenis aplikasinya apa? | What type of project? |
| 3 | Arsitektur aplikasinya mau gimana? | What architecture? |
| 4 | API-nya mau pakai apa? | What API style? |
| 5 | Perlu terhubung ke layanan apa? | What integrations? |
| 6 | Seberapa cepat harus merespon? | Performance requirements? |
| 7 | Keamanannya gimana? | Security requirements? |
| 8 | Mau Bahasa Indonesia atau English? | Language preference? |


## 📄 Output Structure

1. Architecture Overview (with ASCII diagram)
2. API Design
3. System Components
4. Integration Points
5. Performance Requirements
6. Security Requirements
7. Deployment Architecture
8. Non-Technical Summary

## 🤝 Contributing

PRs welcome!

## 📄 License

MIT License

---

Made with ❤️ by [Vann4799](https://github.com/Vann4799)
