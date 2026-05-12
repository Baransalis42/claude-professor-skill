# 🎓 claude-professor-skill

> **Transform Claude into a strict, intelligent university professor** — with structured lecture modes, interactive MCQ widgets, exam simulation, weakness tracking, and exam probability ratings.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Skill](https://img.shields.io/badge/Claude-Skill-blue)](https://claude.ai)
[![Education](https://img.shields.io/badge/Category-Education-green)]()

---

## 🧠 What is this?

`claude-professor-skill` is a **plug-and-play Claude skill** that activates a full university professor persona inside Claude. It is built for students, self-learners, and educators who want AI-powered studying that goes far beyond simple Q&A.

Once activated with the keyword **`lecture me`**, Claude becomes a domain-expert professor capable of:

- 📚 Teaching structured lectures with real academic depth
- 📝 Generating and grading full exams (midterm & final)
- 🔮 Predicting high-probability exam topics
- 💪 Running adaptive practice sessions targeting your weak areas

This is not a generic chatbot prompt. It is a **structured, stateful, interaction-driven skill** with a strict MCQ widget system, memory tracking, and a star-based exam importance rating system.

---

## ✨ Features

### 🎯 4 Core Modes

| Mode | Description |
|------|-------------|
| **1. Lecture Mode** | Professor-style teaching with concept → intuition → example → common mistakes. Ends with MCQ generation. |
| **2. Exam Mode** | Full midterm or final simulation. No answers revealed until full submission. Strict grading. |
| **3. Prediction Mode** | AI identifies high/medium/low probability exam topics using the ⭐ system. |
| **4. Practice Mode** | Adaptive exercises starting easy → hard. Focuses on your weak areas automatically. |

---

### ⭐ Exam Importance Rating System

Every concept is labeled with exam probability so you study smarter:

| Rating | Meaning |
|--------|---------|
| ⭐ | Low probability — good to know |
| ⭐⭐ | Medium probability — study this |
| ⭐⭐⭐ | **HIGH probability — very likely on exams** |

Concepts rated ⭐⭐⭐ are explicitly flagged: *"This concept is very likely to appear in exams."*

---

### 📊 Interactive MCQ Widget System

All multiple-choice questions follow a strict interactive format:

- **Selectable A/B/C/D buttons** — click to answer
- **Immediate color-coded feedback** — ✅ green for correct, ❌ red for incorrect
- **Professor-level explanations** after every answer
- **Previous / Next navigation buttons**
- **Next Question locked** until you answer (no skipping)
- **Full score tracking** and final grade

  Here's what it looks like in action:

  <img width="798" height="636" alt="image" src="https://github.com/user-attachments/assets/f0f7341e-17a8-4a21-b0b3-6e253b36f1aa" />

  The widget highlights your selection in red if wrong and the correct answer in green, followed by a detailed professor-level explanation — instantly, before you move on.


---

### 🧠 Memory & Weakness Tracking System

The professor tracks your performance internally across the session:

| Status | Condition |
|--------|-----------|
| ✅ Strong Topic | Consistently correct answers |
| ⚠️ Weak Topic | Wrong answer recorded |
| 🚨 Critical Weak Area | Repeated mistakes on same concept |

Weak areas are **automatically revisited** and flagged: *"This is one of your weak areas — we need to reinforce it."*

---

## Step 1 — Installation

### Option 1 — Project-level (applies to one project)

1. In your project root, create the folder `.claude/skills/` if it doesn't exist.
2. Copy `professor.md` into `.claude/skills/professor.md`.

### Option 2 — Global (applies to all your projects)

1. Open your global Claude Code config folder:
   - **Windows**: `C:\Users\<you>\.claude\skills\`
   - **macOS / Linux**: `~/.claude/skills/`
2. Copy `professor.md` into that folder.

> If the `skills/` folder does not exist, create it manually.

### Step 2 — Activate

Type exactly:

```
lecture me
```

### Step 3 — Select a Mode

Claude will display:

```
SELECT MODE:
1. Lecture Mode (teach + interactive questions)
2. Exam Mode (generate full exam)
3. Prediction Mode (midterm/final predictions)
4. Practice Mode (exercises only)
```

Select a mode (1–4) and optionally specify a topic.

### Step 4 — Study

Claude will teach, quiz, test, or predict — depending on your mode — using your uploaded course materials or specified subject.

---

## 🔧 Technical Details

- **Activation keyword:** `lecture me`
- **Compatible with:** Claude claude-sonnet-4-20250514, Claude Opus, Claude.ai, Claude Projects
- **Skill type:** Instruction-based prompt skill (no API key required)
- **Interaction model:** Stateful, turn-based, user-gated navigation
- **MCQ rendering:** Button-based with inline color feedback (green/red)
- **Memory scope:** Session-scoped weakness tracking

---

## 🤝 Contributing

Pull requests are welcome. If you have ideas for new modes, better MCQ rendering, or subject-specific improvements — open an issue first to discuss.

---
## 📬 Contact

**Baran Salis** — [@Baransalis42](https://github.com/Baransalis42)
**Emrecan Bektas** — [@emrecanbektas](https://github.com/emrecanbektas)

**Project Link:** — https://github.com/emrecanbektas/claude-professor-skill)

---
## 📄 License

MIT License — free to use, modify, and distribute. See [LICENSE](./LICENSE) for details.

