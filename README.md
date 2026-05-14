# 🎓 AI Study Planner — Multi-Agent System

> *Your personalized AI academic coordination team*

A pipeline of five intelligent agents that transforms your study goals into a structured, week-by-week learning roadmap — complete with curated books, YouTube channels, practice sites, wellness tips, and a motivational send-off. Everything prints beautifully right in your terminal.

---

## 🚀 How It Works

The system chains five specialized agents in sequence, each owning a distinct step of the planning process:

| Agent | What It Does |
|---|---|
| 🔍 **Input Analyzer** | Parses your subject, exam date, daily hours, and weak topics into structured data |
| 📅 **Study Strategy** | Builds a week-by-week roadmap with theory/practice/review time splits |
| 📚 **Resource Recommender** | Curates books, YouTube channels, practice websites, and active learning techniques |
| 🚀 **Motivation & Productivity** | Injects a Pomodoro break schedule, wellness tips, and a personalized motivational quote |
| 📋 **Final Planner** | Compiles everything into a polished terminal display |

---

## 📋 Prerequisites

- Python 3.9+
- An OpenAI API key **or** a Groq API key

---

## 📦 Installation

```bash
pip install langchain langchain-openai langgraph python-dotenv rich
```

---

## ⚙️ Environment Setup

Create a `.env` file in the project root:

```env
# If using OpenAI
OPENAI_API_KEY=your_openai_api_key_here

# If using Groq
GROQ_API_KEY=your_groq_api_key_here
```

---

## 💡 Example Interaction

Run the script and answer four quick prompts:

```
What subject are you studying?          physics
When is your exam/deadline?             May 30
How many hours can you study daily?     8
What are your weak topics? (Optional)   
```

### Sample Output

The agents collaborate in real time and produce a full plan like this:

```
Week 1 — Review and Weak Topic Identification (Apr 30 – May 6)
  • 8 hrs/day  |  Theory (4h) + Practice (3h) + Review (1h)
  • Day 1–2: Mechanics, Electromagnetism, Thermodynamics
  • Day 3–4: Waves, Optics, Modern Physics
  • Day 5–6: Practice problems & past exams
  • Day 7:   Assessment — identify weak spots

Week 2 — Weak Topic Focus (May 7 – May 13)
  • 8 hrs/day  |  Theory (3h) + Practice (4h) + Review (1h)
  • 2–3 days per weak topic, theory + practice mix

Week 3 — Comprehensive Review (May 14 – May 20)
  • 8 hrs/day  |  Theory (2h) + Practice (5h) + Review (1h)
  • Full-syllabus sweep + progress assessment

Week 4 — Final Preparation (May 21 – May 29)
  • 8 hrs/day  |  Theory (1h) + Practice (6h) + Review (1h)
  • Mock exams, timed practice, final review
```

**Resources recommended (Physics example):**

- 📖 *Physics* — Halliday, Resnick & Walker
- 📖 *Fundamentals of Physics* — Halliday, Resnick & Walker
- ▶️ 3Blue1Brown · Crash Course Physics · Physics Girl
- 🌐 Khan Academy Physics · HyperPhysics
- 🗺️ Active technique: Concept Mapping (MindMeister / Coggle)

**Productivity:** Pomodoro schedule (25 min focus → 5 min break → long break every 4 cycles), hydration reminders, and a personalized motivational quote to close out the plan.

---

## 🗂️ Project Structure

```
MultiAgent_StudyPlanner/
├── multi_agent.py   # Core agent pipeline
├── .env             # Your API keys (not committed)
├── .gitignore
└── README.md
```

