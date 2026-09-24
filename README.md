Campus Shuttle — UX Case Study
> **A research-driven campus transportation UX project that moves from observed problem → validated information architecture → prioritized MVP → prototype → usability evaluation → iteration → peer benchmarking → coded prototype.**
This repository contains the complete Campus Shuttle UX Case Study, combining the original Mid-Term work with the subsequent End-Term continuation.
The website is intentionally presented as one continuous case study. The original Mid-Term visual system remains the foundation, and the End-Term work continues directly after the Final MVP rather than appearing as a separate redesign.
---
01 · Project Overview
The problem
Students waiting for the campus shuttle do not always know whether the shuttle is on time, delayed, where it currently is, or whether the schedule has changed.
The research documented a concrete waiting experience at the campus shuttle stop:
Three students were observed at the shuttle stop.
The scheduled shuttle time was 2:15 PM.
The shuttle did not arrive at the expected time.
Students waited and asked about the delay.
One student checked their phone while waiting.
A student described the late shuttle as an ongoing problem.
The shuttle eventually arrived at approximately 2:45 PM.
The project therefore focuses on improving access to clear, timely shuttle information rather than starting with a predetermined digital solution.
Project goal
Design a campus-shuttle information experience that helps students quickly understand:
Current Shuttle Status
Expected Arrival Time
Delay Information
Schedule Change Alerts
These four features became the final Must-Have MVP after the research, card sorting, information architecture, tree testing, and prioritization stages.
---
02 · UX Process
The project follows a research-first UX process:
```text
Problem Space
      ↓
Research
      ↓
Proto Persona
      ↓
Observation
      ↓
User Persona
      ↓
Empathy Map
      ↓
Pain Point
      ↓
User Stories
      ↓
Feature / Content List
      ↓
Card Sorting
      ↓
Information Architecture
      ↓
Tree Test
      ↓
IA Validation
      ↓
MoSCoW + DFV Prioritization
      ↓
Final MVP
      ↓
Wireframing
      ↓
Heuristic Inspection
      ↓
Interactive Prototype
      ↓
Usability Testing
      ↓
Usability Analysis
      ↓
Next Iteration
      ↓
Peer Benchmarking
      ↓
Functional Coded Prototype
      ↓
System Behaviour
      ↓
Final Reflection
```
The sequence matters: solutions are introduced after the research and definition stages rather than being assumed at the beginning.
---
03 · Research & Definition
Research approach
The project began with direct observation and user-oriented research.
The research artifacts include:
Proto Persona
Observation Log
User Persona
Empathy Map
User Journey Map
Core Pain Point
User Stories
Key research direction
The research moved the project from a general transportation problem toward a specific information problem:
> Students need to know **what is happening with the shuttle right now** and **what they should expect next**.
This distinction later influenced the Information Architecture and the final MVP.
---
Observation
The observation was documented objectively rather than treating assumptions as facts.
The recorded shuttle-stop situation showed:
Expected arrival: 2:15 PM
Actual observed arrival: approximately 2:45 PM
Students waited without clear real-time information.
Students sought information from other people and their phones.
The uncertainty itself became part of the user problem.
---
Core pain point
The central issue is not simply that a shuttle can be late.
The larger UX issue is:
> **Students lack timely and understandable information about shuttle status, arrival, delays, and schedule changes while they are waiting.**
---
04 · Information Architecture
Card Sorting
Card sorting was used to understand how participants naturally grouped shuttle-related information.
The resulting structure was used to define the content categories before finalizing the navigation.
Tree Test
A tree test was then used to validate whether users could find information within the proposed structure.
The result informed the final IA rather than assuming that the first structure was automatically correct.
Final Information Architecture
The final IA is centered around four primary user information needs:
```text
Campus Shuttle
│
├── Current Shuttle Status
├── Expected Arrival Time
├── Delay Information
└── Schedule Change Alerts
```
This structure directly supports the final MVP.
---
05 · Prioritization & Final MVP
The project used:
MoSCoW Prioritization
DFV Matrix
The prioritization process identified four Must-Have features.
Final MVP
Must-Have	User need addressed
Current Shuttle Status	Understand whether the shuttle is on time or delayed and where it currently is
Expected Arrival Time	Know when the shuttle is expected to arrive
Delay Information	Understand the delay duration, reason, updated arrival, and freshness of information
Schedule Change Alerts	See when the planned shuttle time changes
The four features form the core of the final prototype and coded experience.
---
06 · Build, Evaluate & Refine
After the Final MVP, the project continued into a build-and-evaluate cycle.
This section is deliberately treated as a continuation of the same case study:
```text
Final MVP
   ↓
Wireframing
   ↓
Heuristic Inspection
   ↓
Interactive Prototype
   ↓
Usability Testing
   ↓
Analysis
   ↓
Next Iteration
```
---
Wireframing
The wireframing stage translated the prioritized MVP into screen-level structures.
The prototype evidence includes screens for:
Current Shuttle Status
Expected Arrival Time
Delay Information
Schedule Change Alerts
Loading State
Error / Information Unavailable State
Schedule Update
The loading state also includes a Cancel action so that the user retains control while information is being retrieved.
---
07 · Heuristic Inspection
A heuristic inspection was performed using Nielsen's usability heuristics.
The supplied inspection specifically checked:
Visibility of System Status
User Control & Freedom
Error Prevention
Finding 01 — Visibility of System Status
Problem: The delay information screen did not initially show when the information was last updated.
Impact: A user could not easily judge how fresh the delay information was.
Fix: Add a Last Updated time.
This makes the freshness of information visible rather than forcing the user to guess.
Finding 02 — User Control & Freedom
Problem: The Expected Arrival loading state did not provide a clear way to leave the operation.
Impact: The user could feel stuck while information was being retrieved.
Fix: Add a Cancel button.
Error Prevention
Error Prevention was considered during inspection, but it was not treated as a confirmed violation without supporting evidence.
---
08 · Interactive Prototype
The interactive prototype represents the main user flow:
```text
Home
 ├── Current Shuttle Status
 ├── Expected Arrival Time
 │       ├── Loading
 │       └── Information unavailable → Try Again
 ├── Delay Information
 └── Schedule Change Alerts
```
The prototype also demonstrates alternative states rather than showing only the ideal successful path.
States represented
Normal information display
Loading
Information unavailable / error
Retry
Cancel
Back navigation
Updated arrival information
Schedule change
---
09 · Usability Testing
The prototype was evaluated through a formal usability-testing round.
Participants
5 participants
Tasks
Participants were asked to perform tasks around the core information needs, including finding:
current shuttle status
expected arrival
delay information
schedule changes
the appropriate action when information is unavailable
Task completion
The documented result was:
> **21 / 25 successful independent task completions = 84%**
This result is treated as the recorded usability-testing outcome for this iteration.
What the result showed
The testing did not simply validate the interface.
It revealed areas where users could still become uncertain, particularly around:
the difference between Current Status and Expected Arrival
the relationship between Delay Information and Schedule Change Alerts
These findings became inputs for the next iteration.
---
10 · Usability Analysis
Finding 01 — Current Status vs Expected Arrival
The testing showed that users could confuse:
where the shuttle is / its current state
when the shuttle is expected to arrive
This suggests that the labels and supporting descriptions need to communicate the distinction more explicitly.
Design implication
The interface should make the difference between:
NOW → current shuttle state
and
WHEN → expected arrival
more immediately understandable.
---
Finding 02 — Delay Information vs Schedule Change
Users could also interpret these two concepts as overlapping.
The distinction is:
Delay Information: explains the current delay and updated arrival context.
Schedule Change Alerts: communicates a change to the planned schedule.
The next iteration therefore focuses on clearer descriptions and stronger information separation.
---
11 · Next Iteration
The next iteration proposes clearer descriptions and stronger differentiation between the information categories.
These are proposed improvements, not claims of a second validated usability round.
The distinction is important:
> A design change can be proposed from a usability finding without claiming that it has already been retested and proven.
---
12 · Peer Benchmarking
Peer benchmarking was completed using the supplied Peer Benchmarking and Final Insights spreadsheet.
The comparison considered:
Domain / Problem
Information Architecture
Must-Have selection
Main User Task
Error / Alternative States
Difference from Campus Shuttle
Why the approach was chosen
What was learned
Peer 01 — Administrative Request Tracking System
Dimension	Record
Peer	Administrative Request Tracking System
Domain / Problem	Reducing uncertainty after students submit administrative requests at Vijaybhoomi University.
IA	Four groups: My Requests, New Request, Updates and Actions, and Help. Card sorting created the groups; tree testing then led to moving Delay Update into My Requests.
Must-Haves	They used MoSCoW, then DFV to compare Expected Completion Date and Progress Timeline. Expected Completion Date became the fourth Must-Have.
Main Task	Track an administrative request: see current status, expected completion, and updates without repeated follow-ups.
Errors / Alternatives	The case study includes Pending Action, Missing Document Alert, Status Update Notification, Comments/Admin Updates, Help/FAQ and Contact Concerned Department. It does not document a specific prototype error-state flow.
Difference	The peer's system focuses on administrative-request tracking and groups progress/time information under My Requests. My project focuses on shuttle information and separates Status, Arrival, Delay and Schedule Change.
Rationale	Tree testing showed that users expected progress and time-related information together, so Delay Update was moved into My Requests.
Learning	IA should follow users' mental models and be changed when testing reveals navigation confusion.
Peer 02 — RouteMate
Dimension	Record
Peer	Peer 2
Domain / Problem	Students who commute from home to college face delays and cancellations in public or college transport, making it difficult to find a reliable backup option and causing late arrival to lectures.
IA	The IA is organized around the commuter’s journey. It starts with Home, then moves through My Commute and Live Status, followed by transport selection at Karjat. Users can compare options, confirm their choice, and track the active journey. Backup Options and SOS provide support, while alerts and alternatives handle delays or cancellations.
Must-Haves	Based on the commuter’s main pain point, focusing on live status, backup options, and handling delays/cancellations.
Main Task	Plan and manage the daily commute to college, check live transport status, choose a suitable last-leg transport option, and switch to a saved backup plan when a delay or cancellation occurs.
Errors / Alternatives	It provides a Loading state while live data is being fetched, an Error state with “Try Again,” “Use Last Status,” and “Back to Home” options, and a Travel Alert when the selected transport is cancelled. Users can then choose an alternative or use their saved backup plan.
Difference	The main difference is that RouteMate focuses on commuter travel reliability and backup planning during delays or cancellations, while my project has a different primary problem and user flow. RouteMate specifically uses Live Status to trigger alternative transport and a Saved Backup Travel Plan.
Rationale	They chose this approach because the main problem is unreliable transport during delays and cancellations. The approach provides live status, alternative transport options, and a saved backup plan so the commuter can continue the journey instead of being left without a dependable option.
Learning	I learned that live-status information should be clear and up to date, and users should always get a chance to review changes before confirming them. Error, loading, and alternative states are also important for helping users recover when something goes wrong.
Peer 03 — SmartSeat
Dimension	Record
Peer	Peer 3
Domain / Problem	Students have no way to know which dining-hall seats are free or claim one in advance, leading to wasted trips and crowding at peak lunch time.
IA	Four main areas: Home/Availability (seat count + booking status), Seat Selection (row → table → seat), Check-in/Timing (countdown, check-in action), and Confirmation. Admin has a separate, structurally distinct dashboard (session control, seat/QR management, analytics).
Must-Haves	Driven by the physical constraints given (24 seats, one lunch window) and by what makes double-booking and no-shows impossible. Real-time sync, server-authoritative timing, and check-in were treated as non-negotiable Must-Haves; the visual floor map and multi-hall support were left as Won't-Have-for-now.
Main Task	Reserve an available seat, check in within the grace window, and use it for a bounded duration before it is released back to the pool.
Errors / Alternatives	Explicit states cover booking-not-open, seat-just-taken conflicts, expired/no-show reservations, invalid or wrong-seat QR scans, and connection loss (with polling fallback). Error messages explain what happened and what to do next, such as choosing another seat after a conflict.
Difference	SmartSeat focuses on dining-hall seat reservation and uses real-time availability, check-in, and timed seat release. My project focuses on campus shuttle information, including current status, expected arrival time, delays, and schedule changes.
Rationale	Because a physical seat can only be occupied by one person at a time and the exhibition demo depends on trust, double-booking prevention and visible system status (open/closed and time remaining) were prioritized over visual polish or extra features.
Learning	Server-authoritative time and locking matter more than UI polish when multiple users interact with the same resource at the same time. Most of the important design decisions were about state and timing, not just layout.
Final insights from the peer sheet
The supplied sheet records the following synthesis:
All three peer projects organize information around the user's main task/problem. Each uses clear functional groups rather than organizing only by internal system features. Testing or real-world constraints influenced the structure.
The peers differed because their core problems and constraints were different: administrative request progress, commuter reliability and backup travel, and dining-hall seat reservation with real-time concurrency. My Campus Shuttle project focuses on quickly finding current status, expected arrival, delay information, and schedule changes.
Peer 1 groups progress/time information under My Requests after tree-testing revealed a mental-model mismatch. Peer 2 uses Live Status to connect delays/cancellations to alternative transport and a saved backup plan. Peer 3 emphasizes server-authoritative timing, locking, check-in and explicit conflict/error states because seats are a shared resource. My IA separates shuttle status, arrival, delay and schedule information as distinct user-facing needs.
I learned that IA should follow the user's mental model and be validated through testing. I also learned that live information needs clear system status and recovery paths, and that alternative/error states should be designed as part of the main experience rather than treated as an afterthought. System constraints can also strongly affect IA and interaction logic.
For the next iteration, I would clarify the Home labels/descriptions for Current Shuttle Status, Expected Arrival Time, and Delay Information because usability testing showed confusion between these features. I would also consider a Report/Support feature as a future opportunity based on participant feedback, without changing the current MVP unless further research supports it.
---
13 · Functional Coded Prototype
The final project includes a coded prototype representation of the shuttle experience.
The front-end experience is based on the supplied HTML/CSS/JavaScript implementation and the project documentation's described Flask/Python backend architecture.
The conceptual flow is:
```text
User
  ↓
Interface
  ↓
Frontend interaction
  ↓
Backend / API
  ↓
Shuttle information
  ↓
Updated interface state
```
The implementation is presented as a prototype rather than claiming a production-grade live shuttle tracking infrastructure.
---
14 · System Behaviour
The coded prototype demonstrates multiple system states.
Normal state
The interface displays available shuttle information such as:
status
location
expected arrival
update time
Loading state
When information is being retrieved:
```text
Loading...
Please wait while arrival information is retrieved.
```
The user can cancel the operation.
Error state
When information cannot be retrieved:
```text
Shuttle Information Unavailable

We couldn't retrieve the latest shuttle information.

Please try again.
```
The user can:
Try Again
Go Back
Schedule update
The interface can communicate a change such as:
```text
Previous time → New time
```
This supports the user's need to understand that the planned shuttle time has changed.
---
15 · Evidence & Design Decisions
The project deliberately distinguishes between:
Observed / researched
Things directly supported by the research, observation, testing, or supplied peer records.
Designed
Interface decisions made from those findings.
Proposed
Potential next-iteration improvements that have not yet been validated through another testing round.
This distinction prevents the case study from presenting design assumptions as research evidence.
---
16 · Repository Structure
```text
Campus-Shuttle-UX-Case-Study/
│
├── index.html
├── style.css
├── README.md
│
└── images/
    ├── card-sort.jpg
    ├── dfv.jpg
    ├── empathy-map.jpg
    ├── features.jpg
    ├── heuristic-fixes-notes.jpg
    ├── heuristic-notes.jpg
    ├── ia.jpg
    ├── journey-map.jpg
    ├── moscow.jpg
    ├── observation-log.jpg
    ├── pain-point-stories.jpg
    ├── proto-persona.jpg
    ├── prototype-alerts.jpg
    ├── prototype-arrival.jpg
    ├── prototype-delay.jpg
    ├── prototype-error.jpg
    ├── prototype-home.jpg
    ├── prototype-loading.jpg
    ├── prototype-status.jpg
    ├── tree-test.jpg
    ├── user-persona-1.jpg
    └── user-persona-2.jpg
```
---
17 · Running the Case Study
This is a static website.
Option 1 — Open locally
Open:
```text
index.html
```
in a browser.
Keep the `images/` folder in the same directory as `index.html`.
Option 2 — VS Code
Open the project folder in VS Code and use a local development extension such as Live Server if required.
The case study does not require a build step for the static presentation.
---
18 · Visual Design System
The final website intentionally continues the original Mid-Term visual language.
Typography
Fraunces — display headings
Public Sans — body and interface text
JetBrains Mono — labels, metadata and technical annotations
Visual language
Warm paper/cream background
Dark ink typography
Blue, teal, ochre and clay accents
Thin borders
Small-radius cards
Structured editorial grids
Evidence-first image presentation
Phase-based navigation
Lightbox image viewing
The End-Term material is therefore not presented as a separate visual redesign.
It is a continuation of the same UX case study.
---
19 · Final Reflection
The project began with an observed waiting problem and developed through a sequence of research and validation activities.
The most important progression was:
```text
Observed uncertainty
        ↓
Research
        ↓
Information needs
        ↓
IA
        ↓
Prioritization
        ↓
MVP
        ↓
Prototype
        ↓
Usability evidence
        ↓
Iteration
        ↓
Benchmarking
        ↓
Coded prototype
```
The project demonstrates that the interface was not chosen first and then justified afterward. The information architecture and feature priorities were progressively shaped through research, testing, and evaluation.
The final result is a continuous UX case study showing the transition from understanding the problem to designing, evaluating, and implementing a solution.
---
Submission Note
This repository is intended as the final combined submission for the Campus Shuttle UX project.
Primary deliverable: `index.html`
Supporting files: `style.css` and `images/`
Research evidence: embedded throughout the case-study sections.
Peer benchmark source: supplied peer-benchmarking spreadsheet.
---
Project
Campus Shuttle — UX Case Study
Scope: Research → IA → Prioritization → MVP → Prototype → Usability Evaluation → Iteration → Peer Benchmarking → Coded Prototype
Format: Responsive HTML/CSS/JavaScript case-study website
