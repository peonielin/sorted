Sorted
---
Your group chat has the ideas — Sorted handles the rest.

This is an autonomous hangout planning app that turns messy group chats into actual plans. It automatically handles scheduling, decision-making, and itinerary creation so no one has to organise. I built this project to explore real-time systems, decision engines, and social UX. The focus is on functionality and behaviour rather than polish.

📦 Tech Stack
---
* Vite
* React.js
* TypeScript
* Node.js (Express)
* PostgreSQL
* Socket.IO
* CSS

🦄 Features
---
Here’s what you can do with Sorted:

* **Create a hangout**: Start with a rough idea (e.g. “dinner this weekend”) and invite your group via a link.
* **Mark availability**: Tap simple time blocks (morning, arvo, evening, night) so Sorted can find the best overlap.
* **Auto scheduling**: Sorted automatically finds and locks the best time when enough people are available.
* **Planning chat**: A lightweight chat focused only on decisions, not social noise (inline polls, system updates).
* **Auto decision engine**: Detects suggestions, agreement, and rejection in chat and automatically pins decisions.
* **Dynamic updates**: If the group changes direction, Sorted updates the plan automatically.
* **Smart interventions**: Handles split decisions, non-responsive users, and duplicates with polls and nudges.
* **System personality**: Human-like messages such as “Looks split 👀”, “Almost there…”, “Just waiting on Ryan”.
* **Dynamic itinerary**: Generates a structured plan (time, venue, who’s coming, who’s bringing what, checklists).

👩‍🍳 The Process
---
I started by focusing on the core problem — plans dying in group chats — and designed Sorted around removing all coordination effort.

First, I built the availability system so users could respond in under 10 seconds using simple time blocks instead of complex calendars.

Next, I built the scheduling engine that finds overlap and automatically locks in a time when enough people are available.

Then I built the decision engine, which detects suggestions, agreement, and rejection from chat messages and assigns confidence scores to decide when something should be pinned.

After that, I implemented real-time updates using Socket.IO so all users see changes instantly.

I then added the auto-pin system so decisions build themselves dynamically as the conversation evolves.

Finally, I built the itinerary generator, which converts pinned decisions into structured plans depending on the type of hangout (dinner, picnic, house party, etc.), and added a personality layer to make the system feel more human.

📚 What I Learned
---
A lot of things around systems thinking, but mainly:

* How to turn human behaviour (agreement, disagreement, indecision) into logic
* How to design systems instead of individual features
* How edge cases define product quality (split decisions, non-response, conflicts)
* How real-time systems work using WebSockets
* How small UX details (like tone and nudges) change user behaviour
* That simple rule-based systems can go very far without heavy AI

💭 What Can Be Improved?
---
* Add AI-based intent detection for better decision accuracy
* Integrate Google / Apple Calendar
* Add venue recommendations (restaurants, activities)
* Improve UI polish and responsiveness
* Add expense splitting
* Add user preference learning (food, timing, etc.)
* Improve notification timing and personalization

🚦 Running the Project
---
To run Sorted locally:

* Clone the repository
* Run `npm install`
* Run `npm run dev`
* Open `http://localhost:3000`

🍿 Final Thought
---
Sorted isn’t just a planner.

It’s an attempt to answer:

> What if plans could organise themselves?
