# Lexi

**A browser-based learning prototype built around active recall, graduated hints, and retrieval tracking.**

**[Try Lexi →](https://leahlizrp.github.io/lexi/)**
<img width="867" height="877" alt="download" src="https://github.com/user-attachments/assets/841ce012-fbc2-4adc-86d9-04ad700f3484" />
*Try an acronym, learn its meaning, then practice recalling it with graduated hints.*

Lexi started as a way to learn AI terminology more effectively and is evolving into an experiment in how AI can support long-term, adaptive learning.

## What is Lexi?

Lexi is a learning system designed to do more than tell you whether an answer is right or wrong.

The current prototype helps learners try an acronym, learn what it means, and practice recalling its full meaning. It distinguishes between unassisted recall, hint-assisted recall, and revealed answers.

The larger goal is to expand beyond terminology into AI concepts, frameworks, tools, and applied reasoning, with adaptive learning and reassessment over time.

## Why I'm Building It

While learning AI, I found that recognizing a term wasn't the same as actually understanding or being able to retrieve it.

I wanted a system that could notice the difference.

Lexi grew from that problem: create a learning experience that adapts to what the learner actually knows, where they wobble, what kind of help works, and what needs to return later.

## How Learning Works

The current prototype follows three steps:

1. **Try:** Choose what an acronym stands for, or open its lesson for help.
2. **Learn:** Read the meaning and memory tip, then make a correct multiple-choice selection before adding the acronym to drills. The first five starter lessons also include explanations and examples.
3. **Drill:** Recall the full meaning from memory. Ask for up to two progressively stronger hints before revealing the answer.

Completed drills are recorded as **Unassisted**, **Hinted**, or **Taught**. Lessons and multiple-choice attempts do not add to these counts. An acronym being ready for drills means it has been introduced and checked; it does not mean it has been mastered.

## Current Features

The current prototype includes:

- 250 acronyms covering AI, machine learning, statistics, computing, and related technical topics
- A try → learn → drill flow
- Correct / Partial / Incorrect feedback during recall practice
- Acceptance of small spelling slips
- Two graduated hints before an answer can be revealed
- Unassisted, hinted, and taught retrieval tracking
- Browser-saved drill history and unlocked acronyms
- Repeat practice through the unlocked collection

## Getting Started

Open `index.html` in a web browser. No installation or account is required.

Progress is saved locally in the browser on that computer. Keep using the same file and browser to continue your practice. Progress does not sync across browsers or devices, and clearing browser data removes it.

If browser storage is unavailable, Lexi shows a notice and keeps progress for the current session only.

## Public Prototype Cleanup

This version removes a personalized study-session reference from the Reinforcement Learning hint and standardizes word-count formatting in the first 16 hints. The visual design and learning behavior are unchanged.

It also starts a fresh tracker using `lexi-history-v2` and `lexi-understood-v2`. Progress saved under the earlier v1 keys is left intact but is no longer loaded. New practice is saved under the v2 keys and continues across visits in the same browser.

## What I'm Experimenting With

Lexi is also a sandbox for exploring questions around human-centered AI and learning:

- When should an AI help versus let someone struggle?
- How much assistance improves learning without replacing retrieval?
- What signals actually indicate mastery?
- How should difficulty adapt over time?
- How can an AI learning system explain why it is changing its behavior?
- How can learner trust and control be preserved as the system becomes more adaptive?

The current prototype uses a fixed acronym dataset and browser-based learning logic. It does not connect to an AI model or automatically adapt difficulty based on performance.

## Roadmap

Future directions include:

- Expanding beyond acronyms/terminology into broader AI concepts
- Concept deep dives and applied questions
- Spaced reassessment after successful recall
- Retrieval-speed tracking
- Adaptive session generation and difficulty
- Mastery progression and more sophisticated mastery modeling
- Cross-topic learning
- Improved learner progress visualization
- Exploring multiple learning/assessment agents

## Current Status

**Early prototype / active development.**

Lexi currently works as a browser-based prototype and is being actively tested and expanded as I learn more about AI, HCI, adaptive learning, and conversational system design.

This repository will document both the system and what I learn while building it.
