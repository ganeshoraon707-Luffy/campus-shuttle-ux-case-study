<div align="center">
🚌 Campus Shuttle
From an uncertain wait → to an informed decision.
A UX case study exploring how students experience campus shuttle delays —  
from field observation → research → information architecture → prototyping → usability testing → iteration.
<br>
![UX Case Study](https://img.shields.io/badge/UX-Case%20Study-33513A?style=for-the-badge)
![HTML](https://img.shields.io/badge/HTML-Only-8C4B3A?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-Interface-2C4666?style=for-the-badge&logo=css3&logoColor=white)
![Usability](https://img.shields.io/badge/Usability-84%25-8A6A24?style=for-the-badge)
<br>
🔗 Live Case Study:  
https://ganeshoraon707-luffy.github.io/campus-shuttle-ux-case-study/
📦 Repository:  
https://github.com/ganeshoraon707-Luffy/campus-shuttle-ux-case-study
</div>
---
🚌 The Project
Students waiting for a campus shuttle often don't know whether the shuttle is coming, when it will arrive, or whether the schedule has changed.
This project investigates that uncertainty and develops a web-based shuttle information experience around the needs uncovered during research.
> **The goal wasn't to start with an app.**  
> The goal was to understand the user's problem first, then determine what information and interactions were actually needed.
---
📌 Project Snapshot
	
🎯 Domain	Campus Transportation / UX
👤 Focus	Students waiting for campus shuttle services
🔎 Approach	Research-led UX process
🧪 Usability testing	25 task attempts
✅ Completed	21
📈 Completion rate	84%
💻 Final format	HTML + CSS functional prototype
---
🔎 01 — The Problem
What was observed?
At the shuttle stop, students were waiting for a shuttle scheduled to arrive at 2:15 PM.
The shuttle arrived at approximately 2:45 PM.
That created a simple but important UX problem:
The user was waiting — but didn't know what was happening.
The research therefore focused on questions such as:
🕐 When will the shuttle arrive?
📍 Where is it right now?
⚠️ Is it delayed?
🔔 Has the schedule changed?
❓ What should the student do while waiting?
---
🧭 02 — UX Process
The project followed a research-first process rather than jumping directly into interface design.
```text
OBSERVE
   ↓
UNDERSTAND USERS
   ↓
DEFINE PAIN POINTS
   ↓
USER STORY
   ↓
JOURNEY MAP
   ↓
CARD SORTING
   ↓
TREE TEST
   ↓
INFORMATION ARCHITECTURE
   ↓
WIREFRAMES
   ↓
MVP
   ↓
HEURISTIC INSPECTION
   ↓
INTERACTIVE PROTOTYPE
   ↓
USABILITY TESTING
   ↓
ITERATION
   ↓
FUNCTIONAL PROTOTYPE
```
🧠 Research → Structure → Interface → Validation
The interface was developed only after the research and information-architecture stages.
---
⭐ 03 — Final MVP
The research led to four core pieces of information.
🚌 Feature	What the user needs
Current Shuttle Status	Know whether the shuttle is currently running
Expected Arrival Time	Know when it is expected
Delay Information	Understand whether the shuttle is delayed and why
Schedule Change Alerts	Know when an important schedule change occurs
These became the foundation of the prototype.
---
🎨 04 — From MVP → Prototype
The MVP was translated into a set of screens covering the main shuttle journey.
Prototype flow
```text
🏠 Home
   ↓
🚌 Current Status
   ↓
⏱ Expected Arrival
   ↓
⚠️ Delay Information
   ↓
🔔 Schedule Alerts
```
Additional states were also considered:
```text
⏳ Loading State
        ↓
❌ Error State
```
Screens represented in the prototype
Screen	Purpose
🏠 Home	Entry point and shuttle overview
🚌 Status	Current shuttle status
⏱ Arrival	Expected arrival information
⚠️ Delay	Delay reason and updated information
🔔 Alerts	Schedule changes
⏳ Loading	System feedback while information loads
❌ Error	Handling unsuccessful requests
---
🧪 05 — Heuristic Inspection
The prototype was inspected using usability heuristics to identify interaction and feedback problems.
👀 Visibility of System Status
Issue
The initial Delay Information screen did not clearly communicate when its information had last been updated.
Iteration
The screen was updated to show:
Updated arrival information
Delay reason
Last updated time
This makes the freshness of the information visible to the user.
---
🎛 User Control & Freedom
Issue
The initial Expected Arrival loading state did not provide a clear way for the user to leave the operation.
Iteration
A Cancel action was added so the user has control while waiting for the operation to complete.
---
🛡 Error Prevention
Error Prevention was also inspected.
However, the project documentation does not treat it as a confirmed heuristic violation because the available evidence did not support that conclusion.
That distinction was kept intentionally.
---
👥 06 — Usability Testing
The prototype was evaluated through task-based usability testing.
Results
	Result
🧪 Task attempts	25
✅ Successful completions	21
📊 Completion rate	84%
What this means
The testing provided evidence about how participants interacted with the prototype and where the experience could be improved.
The results were then used to inform the next iteration rather than treating the first prototype as final.
---
🔁 07 — Iteration
The design process continued after testing.
```text
Prototype
   ↓
Heuristic Inspection
   ↓
Usability Testing
   ↓
Observed Issues
   ↓
Design Changes
   ↓
Refined Prototype
```
The important shift was from:
> **“Does the screen look good?”**
to:
> **“Does the interface help the user complete the task with less uncertainty?”**
---
👥 08 — Peer Benchmarking
Peer projects were reviewed to understand how other student projects approached:
Information architecture
Navigation
Feature grouping
Presentation of project decisions
UX documentation
The benchmarking stage was used as a reference point for evaluating the structure of the work.
---
💻 09 — Functional Prototype
The final implementation is a lightweight HTML + CSS prototype.
It presents the researched information architecture and interface decisions as a working web page.
System behaviour represented
```text
USER
 ↓
Select shuttle information
 ↓
SYSTEM STATE
 ├── Current status
 ├── Expected arrival
 ├── Delay information
 ├── Schedule alerts
 ├── Loading
 └── Error
```
The implementation focuses on communicating the interaction states clearly rather than presenting the project as a production transportation system.
---
🧰 10 — Built With
Tool / Technology	Use
🌐 HTML	Page structure and content
🎨 CSS	Visual design and responsive layout
🧠 UX Research	Understanding user behaviour
🗂 Information Architecture	Organising shuttle information
🧪 Usability Testing	Evaluating the prototype
📝 GitHub	Version control and project hosting
Visual design language
The case-study site uses an editorial, paper-like visual system:
`#EEE8DA` · `#E4DCC8` · `#F8F4EA` · `#23241F`
with supporting accents:
`#33513A` · `#2C4666` · `#8C4B3A` · `#8A6A24` · `#2E5C57`
Typography combines:
Fraunces — display / editorial headings
Public Sans — interface and body text
JetBrains Mono — technical / metadata elements
---
📁 11 — Project Structure
```text
campus-shuttle-ux-case-study/
│
├── index.html
├── style.css
│
├── images/
│   ├── heuristic-notes.jpg
│   ├── heuristic-fixes-notes.jpg
│   ├── prototype-home.jpg
│   ├── prototype-status.jpg
│   ├── prototype-arrival.jpg
│   ├── prototype-delay.jpg
│   ├── prototype-alerts.jpg
│   ├── prototype-loading.jpg
│   └── prototype-error.jpg
│
└── README.md
```
> Image filenames should match the paths used by `index.html` exactly, including capitalization and file extension.
---
🚀 12 — Run Locally
Clone the repository:
```bash
git clone https://github.com/ganeshoraon707-Luffy/campus-shuttle-ux-case-study.git
```
Open the project:
```bash
cd campus-shuttle-ux-case-study
```
Then open:
```text
index.html
```
in a browser.
No backend or package installation is required for the HTML/CSS prototype.
---
🌐 13 — Live Project
<div align="center">
🚌 Campus Shuttle UX Case Study
Observe → Understand → Structure → Prototype → Test → Iterate
<br>
<a href="https://ganeshoraon707-luffy.github.io/campus-shuttle-ux-case-study/">
<img src="https://img.shields.io/badge/VIEW%20LIVE%20CASE%20STUDY-33513A?style=for-the-badge" alt="View Live Case Study">
</a>
 
<a href="https://github.com/ganeshoraon707-Luffy/campus-shuttle-ux-case-study">
<img src="https://img.shields.io/badge/VIEW%20SOURCE%20CODE-2C4666?style=for-the-badge" alt="View Source Code">
</a>
</div>
---
<div align="center">
🚌 From waiting without information
→ to waiting with context.
Campus Shuttle UX Case Study
</div>
