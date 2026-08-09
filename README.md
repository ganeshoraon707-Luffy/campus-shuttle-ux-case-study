# 🚌 Campus Shuttle — UX/UI Case Study

> **Understanding the broken experience before designing the solution.**

A research-driven UX/UI case study focused on the **campus shuttle waiting experience** and the uncertainty students face when shuttle timings are delayed or changed.

This project follows a structured UX process from **Empathy & Definition → Ideation & Evaluation → Prioritization**, using real user research, observation, card sorting, information architecture, tree testing, MoSCoW prioritization, and DFV analysis.

---

## 🌐 Project

### 🎨 UX Case Study Website

**Campus Shuttle — UX Research & Information Architecture**

The complete case study is presented as a single responsive webpage built using:

- HTML5
- CSS3

> **Note:** This project is a UX case study and validated design blueprint. It is **not a fully functional shuttle-tracking application**.

---

# 🎯 Project Overview

The project began with a simple question:

> **What happens when students are waiting for a campus shuttle and it doesn't arrive when expected?**

Instead of immediately designing an app, the project followed a **research-first approach**.

The process focused on understanding:

- What students actually do
- What they say
- What they may be experiencing
- Where the journey breaks
- What information they need
- How they naturally organize that information
- Whether the proposed information architecture is understandable
- Which features should be prioritized

---

# 🧠 UX Process

```text
┌───────────────────────────────┐
│  PHASE 1 — EMPATHIZE & DEFINE │
└───────────────┬───────────────┘
                ↓
       Problem Space
                ↓
         Proto Persona
                ↓
          Observation
                ↓
         User Persona
                ↓
          Empathy Map
                ↓
         Journey Map
                ↓
           Pain Point
                ↓
          User Stories

┌───────────────────────────────┐
│  PHASE 2 — IDEATE & EVALUATE  │
└───────────────┬───────────────┘
                ↓
        Feature Generation
                ↓
           Card Sorting
                ↓
      Information Architecture
                ↓
           Tree Testing
                ↓
          IA Validation

┌───────────────────────────────┐
│  PHASE 3 — PRIORITIZATION     │
└───────────────┬───────────────┘
                ↓
         MoSCoW Analysis
                ↓
            DFV Matrix
                ↓
          Final MVP Scope
```

---

# 🔎 Phase 1 — Empathize & Define

The first phase focused entirely on **understanding the user before thinking about solutions**.

### Research activities

- Problem-space identification
- Proto-Persona
- User observation
- User Persona
- Empathy Map
- User Journey Map
- Emotion Line
- Pain Point identification
- User Stories

### Observation

The observation was conducted using a **CCTV-style approach**:

> Observe what the users do and hear without adding assumptions to the observation itself.

This helped prevent premature conclusions and solution bias.

---

# 👤 User Understanding

The research was translated into:

### Proto-Persona
An initial representation based on assumptions before research.

### User Persona
A research-based representation of the common user characteristics, behaviours, needs, and frustrations identified during research.

### Empathy Map

The experience was synthesized through:

- **Says**
- **Thinks**
- **Does**
- **Feels**

### Journey Map

The complete experience was mapped across different stages to identify changes in behaviour and emotion.

The **lowest point of the emotional journey** helped identify the core pain point.

---

# 💢 Core Pain Point

The research revealed that students experience **uncertainty and frustration when the campus shuttle does not arrive according to its scheduled time and they lack reliable information about its current status or schedule changes.**

The pain point was defined **before proposing the solution**.

---

# 📝 User Stories

The identified pain point was translated into user-centered requirements using the standard format:

> **As a [user], I want [goal], so that [benefit].**

These User Stories became the foundation for generating potential features.

---

# 💡 Phase 2 — Ideate & Evaluate

After understanding the user, the project moved into information and feature exploration.

### Feature Generation

A total of **20 candidate features/content items** were generated from the identified User Stories.

These were not automatically treated as final features. They were evaluated through subsequent UX research methods.

---

# 🃏 Card Sorting

An **Open Card Sort** was conducted with:

### 👥 11 participants

Participants organized the 20 information items according to how they naturally understood and grouped them.

The resulting patterns were used to inform the Information Architecture.

### Why Card Sorting?

> To understand the users' mental model instead of imposing a structure based only on the designer's assumptions.

---

# 🏗️ Information Architecture

The Card Sort findings were translated into a **Version 1 Information Architecture**.

The IA focused on:

- Clear information grouping
- Findability
- Logical hierarchy
- User-centered organization

---

# 🌳 Tree Testing

The V1 Information Architecture was evaluated using a Tree Test.

### Participants

**5 students**

### Tasks

Participants were asked to find information such as:

- Next shuttle arrival
- Shuttle delay information
- Routes and stops
- Shuttle rules
- Reporting a shuttle problem

### Result

**5/5 participants successfully completed all 5 tasks.**

That means:

> **25/25 task attempts were successful.**

No major structural changes were required because the V1 Information Architecture was successfully understood by all tested participants.

---

# 📊 Phase 3 — Prioritization

After generating and evaluating the possible features, the next step was determining what should actually be prioritized.

Two prioritization methods were used:

### MoSCoW

- 🔴 **Must Have**
- 🟠 **Should Have**
- 🟡 **Could Have**
- ⚪ **Won't Have**

Only **4 features** were selected as Must-Haves.

### DFV

The two closely competing features were evaluated using:

- **Desirability**
- **Feasibility**
- **Viability**

---

# 🏆 DFV Result

| Feature | Desirability | Feasibility | Viability | Total |
|---|---:|---:|---:|---:|
| Shuttle Arrival Alerts | 5 | 4 | 5 | **14** |
| **Schedule Change Alerts** | **5** | **5** | **5** | **15** |

### 🥇 Winner: Schedule Change Alerts

User feedback indicated that knowing about schedule changes in advance would help students **plan their day and adjust their travel accordingly**.

---

# 🚀 Final MVP Scope

Based on the complete UX process, the final four Must-Have features were:

| Priority | Feature |
|---|---|
| ⭐ Must Have | Current Shuttle Status |
| ⭐ Must Have | Expected Arrival Time |
| ⭐ Must Have | Delay Information |
| ⭐ Must Have | Schedule Change Alerts |

These features represent the **prioritized MVP scope**, rather than a fully implemented application.

---

# 🛠️ Technology

This case-study website was created using only:

```text
HTML5
CSS3
```

### No JavaScript
### No React
### No Bootstrap
### No Tailwind
### No external UI framework

The webpage is designed as a **single scrolling UX case study** containing the research evidence, maps, diagrams, findings, IA, evaluation, and prioritization.

---

# 📁 Repository Structure

```text
campus-shuttle-ux-case-study/
│
├── 📄 index.html
├── 🎨 style.css
├── 📖 README.md
│
└── 📁 images/
    ├── observation-log.jpg
    ├── proto-persona.jpg
    ├── user-persona.jpg
    ├── empathy-map.jpg
    ├── journey-map.jpg
    ├── user-stories.jpg
    ├── features.jpg
    ├── card-sort.jpg
    ├── information-architecture.jpg
    ├── tree-test.jpg
    ├── moscow.jpg
    └── dfv.jpg
```

---

# ♿ Accessibility

The case-study webpage follows basic accessibility practices including:

- Semantic HTML
- Descriptive image `alt` attributes
- Clear heading hierarchy
- Readable typography
- Responsive layout
- Keyboard-friendly navigation
- High information clarity

Hand-drawn research artefacts are preserved as image evidence and embedded using HTML `<img>` elements with descriptive alternative text.

---

# 🎓 Academic Context

This project was developed as part of a **UX/UI Design examination**.

The project follows a structured research-first methodology:

> **Understand the user → Define the problem → Generate requirements → Organize information → Evaluate the structure → Prioritize features**

The primary objective was **not to build a complete application**, but to demonstrate a methodical UX process supported by research and evidence.

---

# 💭 Key Learning

The biggest takeaway from this project was:

> **Good UX does not begin with a screen. It begins with understanding the person using it.**

The project reinforced the importance of:

- Research before solutions
- Observation without assumptions
- Empathy before ideation
- User-centered information architecture
- Testing assumptions with real users
- Evidence-based prioritization

---

# 👨‍💻 Author

**Ganesh Oraon**

B.Tech — Artificial Intelligence & Machine Learning

Vijaybhoomi University

---

## ⭐ Project Philosophy

> **Don't design what you think users need.  
> Understand what they actually need first.**
