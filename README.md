# Tutor_bot
# Beacon — AI Learning Companion

**SDG 4: Quality Education** — A personalized AI tutor chatbot built to help students who don't have access to a private tutor at home get clear, level-appropriate explanations, practice quizzes, and curated learning resources, anytime.

> Live demo: open `index.html` in any browser. No installation, no build step, no server required.

---

## 1. Problem Statement

Hundreds of millions of students worldwide lack consistent access to one-on-one academic support. A child who falls behind in class often has no one at home who can explain a concept a different way, no one to check whether they actually understood it, and no way to know what to study next. This gap is worst for students in low-income households, rural areas, and overcrowded classrooms, where teacher-to-student ratios make individual attention nearly impossible. Left unaddressed, small gaps in understanding compound over school years into large learning gaps, dropout risk, and reduced life opportunities.

## 2. Project Objective

Beacon's objective is to give any student with a browser access to a patient, always-available tutor that:
- Explains concepts at a level the student chooses (Beginner / Intermediate / Advanced)
- Lets the student test their understanding immediately through quizzes
- Recommends free, high-quality resources to keep learning after the chat ends
- Tracks progress so the student (or a parent/teacher) can see what's working

## 3. How It Works

Beacon runs entirely client-side as a single HTML file:
- **Offline demo mode** (default): a built-in knowledge base answers common questions across Math, Science, English, and Computer Science, with three difficulty-tuned versions of every explanation.
- **Live AI mode** (optional): if a student enters their own Anthropic API key in Settings, Beacon calls the Claude API directly from the browser for open-ended, unlimited tutoring instead of the fixed demo bank.

This two-mode design means the project **works immediately for grading/demo purposes with zero setup**, while also showing a real path to a production-grade AI integration.

## 4. Features

- **Tutor Chat** — ask any question, get a level-matched explanation, with quick-start suggested questions per subject.
- **Practice Quiz** — auto-generated 5-question quizzes per subject with instant grading and explanations for every answer.
- **My Progress** — quiz history, average score, strongest subject, and a "session streak" star tracker.
- **Resources** — curated free resources (Khan Academy, freeCodeCamp, CS50, PhET, Purdue OWL, etc.) matched to the selected subject.
- **Settings** — optional API key for live AI responses; otherwise runs fully offline.

## 5. Technology Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | Custom CSS (CSS variables / design tokens, no framework) |
| Logic | Vanilla JavaScript (no build tools, no dependencies) |
| Fonts | Google Fonts (Fraunces, Inter, IBM Plex Mono) |
| Optional AI | Anthropic Claude API (`claude-sonnet-4-6`) via direct browser fetch |

No backend, database, or package installation is required — this was a deliberate choice so any student, teacher, or grader can run the project by double-clicking `index.html`.

## 6. Running the Project

1. Clone or download this repository.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari).
3. That's it — the demo knowledge base, quizzes, and resources work immediately.
4. *(Optional)* To enable live AI chat: go to **Settings**, paste an Anthropic API key, click **Save key for this session**.


## 8. Future Scope

- Mobile app version (React Native / Flutter) for offline access without a laptop
- Teacher dashboard to view aggregated student progress across a classroom
- Speech-to-text input for younger learners or students with limited literacy
- Multilingual support so the tutor can explain concepts in a student's first language
- Adaptive difficulty that automatically adjusts level based on quiz performance
- Persistent accounts (with a backend) so progress survives across devices and sessions


