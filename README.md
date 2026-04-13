Sorted
**An autonomous hangout planning app that turns messy group chats into actual plans.**

Sorted automatically handles scheduling, decision-making, and itinerary creation so no one has to organise. I built this project to explore real-time systems, decision engines, and social UX. The focus is on functionality and behaviour rather than polish.
---
📦 Tech Stack
- Vite  
- React.js  
- TypeScript  
- Node.js (Express)  
- PostgreSQL  
- Socket.IO  
- CSS  
---
🕶️ Features

Here’s what you can do with Sorted:

### Create a Hangout
Start with a rough idea (e.g. “dinner this weekend”) and invite your group via a link.
---
### Mark Availability
Tap to mark when you’re free using simple time blocks:
- Morning  
- Afternoon  
- Evening  
- Night  

Sorted finds the best overlap automatically.
---
### Auto-Scheduling
No one has to pick a time.  
Sorted detects the best slot and locks it in when enough people are available.

---

### Planning Chat (Purpose-Built)
A lightweight chat designed for decisions, not conversation:
- Inline polls  
- System updates  
- No read receipts or typing indicators  

---

### Auto Decision Engine
Sorted listens to the chat and:
- Detects suggestions (“let’s do BBQ”)  
- Tracks agreement (“keen”, “I’m in”)  
- Identifies rejection (“too far”, “nah”)  

Then automatically pins decisions and updates them if the group changes direction.

---

### Smart Interventions
When things get messy, Sorted steps in:

- Split decision → auto poll  
- No responses → nudges users  
- One person spamming → ignored  
- Duplicate plans → surfaced  

---

### System Personality
The app feels human with subtle nudges:

- “Looks split 👀”  
- “Almost there…”  
- “Just waiting on Ryan”  

This keeps momentum without forcing users.

---

### Dynamic Itinerary
Sorted turns decisions into a structured plan:

- Time & location  
- Who’s coming  
- Who’s bringing what  
- Checklists (for picnics, etc.)  

Adapts based on the type of hangout.

---

## 👩🏽‍🍳 The Process

I started by focusing on the **core problem** — plans dying in group chats — and designed the system around removing coordination effort completely.

First, I built the **availability system**, allowing users to respond in under 10 seconds using simple time blocks instead of complex calendars.

Next, I implemented the **scheduling engine**, which calculates overlap and automatically locks in a time when enough people are available.

After that, I worked on the **decision engine**, which is the core of the product. It processes chat messages to detect suggestions, agreements, and rejections, then assigns confidence scores to determine when a decision should be pinned.

I then built the **real-time chat system** using WebSockets so that decisions, messages, and updates sync instantly across users.

Once decisions could be tracked, I created the **auto-pin system**, allowing the plan to build itself dynamically as the conversation evolves — including handling reversals and changing opinions.

From there, I developed the **itinerary generator**, which converts pinned decisions into structured blocks depending on the type of hangout (e.g. dinner vs picnic).

Finally, I added the **system personality layer**, introducing small, context-aware messages to guide users through indecision and increase engagement.

Throughout the process, I prioritised behaviour and system logic over UI polish to validate the core concept.

---

## 📚 What I Learned

### 🧠 Decision Systems & Logic
Building the decision engine taught me how to model human behaviour (agreement, disagreement, indecision) into structured logic using scoring systems and thresholds.

---

### ⚖️ Handling Edge Cases
I learned that edge cases define the product:
- Split decisions  
- Non-responsive users  
- Conflicting inputs  

Designing for these made the system feel reliable.

---

### 🔄 Real-Time Systems
Using Socket.IO helped me understand how to manage live updates across multiple users, especially when state changes frequently.

---

### 🧩 System Design Thinking
Instead of building features, I had to think in systems:
- Scheduling system  
- Decision system  
- Itinerary system  

Each part needed to work independently and together.

---

### 🎭 Product Experience
The personality layer showed me how small UX details (like nudges and tone) can significantly impact user behaviour and engagement.

---

### 📉 Simplicity vs Intelligence
I learned that a simple rules-based system (keywords + scoring) can achieve 80% of the value without needing heavy AI.

---

## 💭 How can it be improved?

- Add AI-based intent detection for more accurate decisions  
- Integrate with Google/Apple Calendar  
- Add venue recommendations (restaurants, activities)  
- Improve UI/UX polish and responsiveness  
- Add expense splitting  
- Introduce user preferences (favourite cuisines, times)  
- Improve notification system (timing + personalisation)  

---

## 🚦 Running the Project

To run the project locally:

### 1. Clone the repository
```bash
git clone https://github.com/your-repo/sorted.git
cd sorted
