---
title: "Rebuilding Marble Solitaire with Gemini: My First Experience with an Agentic AI in Android Studio"
slug: "rebuilding-marble-solitaire-with-gemini-my-first-experience-with-an-agentic-ai-in-android-studio"
description: |
  The era of AI-assisted coding is progressing. At first, working with AI meant copy-pasting suggestions from a chatbot into your IDE—useful, but clumsy. Now, with Gemini integrated into Android Studio, I experienced a glimpse of what the future of sof...
date: 2025-09-23
updated: 2025-09-23
status:
  - published
reading_time: 5
cover_image: "/assets/img/blog/2025-09-23-rebuilding-marble-solitaire-with-gemini-my-first-experience-with-an-agentic-ai-in-android-studio/cover.png"
---
The era of AI-assisted coding is progressing. At first, working with AI meant copy-pasting suggestions from a chatbot into your IDE—useful, but clumsy. Now, with Gemini integrated into Android Studio, I experienced a glimpse of what the future of software development might look like: an agentic coding assistant that can see your project, understand its structure, and directly make changes across code and configuration files. It’s a promising leap forward, even if the technology still causes plenty of developer frustration along the way.

---

### What Makes an AI *Agentic*?

The value of an agentic assistant lies in context and interaction. Rather than blindly generating snippets, Gemini continuously reads the state of your project, reasons about it, and applies changes itself. This bi-directional interaction between the AI’s understanding, its suggestions, and its direct implementation makes it feel less like autocomplete and more like pairing with a junior developer who knows their way around the project. In practice, this meant I could ask Gemini to set up a project structure for phone, Wear OS, and Android TV, and it handled the boilerplate with minimal intervention from me.

---

### Reviving an Old Game Across Platforms

For my test project, I chose an old app: peg solitaire. The game is simple but challenging: you move by jumping one marble over another, removing the jumped piece, on a cross-shaped board. There’s no opponent, just the puzzle itself, with the goal of ending with a single marble in the center.

While the phone and Wear OS versions were straightforward, Android TV introduced new complexity. Without touch controls, interaction had to be rethought entirely for the d-pad remote. This required defining explicit states: moving a selection, picking up a marble, choosing a jump direction, and executing the move. Impressively, Gemini handled the development of this navigation model without my stepping in—a task that would have been tedious to wire up by hand.

---

### Where Things Fell Apart

The excitement wasn’t without setbacks. I had hoped to ship the phone, Wear OS, and TV versions together in the same app bundle under a single versionCode. Gemini agreed that this was possible and confidently generated step-by-step instructions for how to achieve it. Unfortunately, those instructions turned out to be hallucinations.

I wasted significant time following these false leads. I restructured the project into libraries, creating dynamic features and later build flavors, and pushing uploads to the Play Store only to discover, each time at the very last minute, that none of it worked. This is the double-edged sword of today’s AI tools: they’re persuasive and helpful up to a point, but they can also lead you deep into dead ends.

---

### Looking Ahead

Despite the frustration, the potential is obvious. An AI that can work directly inside your IDE, understand context, and manage files and configurations is far more powerful than one that only outputs code snippets. But cloud-based assistants come with tradeoffs. I’d prefer not to send my code off-device, and my local machine has sufficient memory available for handling larger projects.

That’s why for my next experiment, I plan to try a local, offline agentic assistant—something like [Continue.dev](http://Continue.dev), which integrates with IntelliJ. If Gemini showed me the promise of this new paradigm, a local tool might show me its true potential.

[Info Page](https://arnodenhond.com/marblesolitaire)

[Google Play](https://play.google.com/store/apps/details?id=arnodenhond.marblesolitairelite)

[GitLab](https://gitlab.com/arnodenhond/marblesolitaire)
