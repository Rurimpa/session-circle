---
name: session-circle
description: Open a "circle," a discussion among two or three Claude Code sessions that are already running, connected with SendMessage. Use when the user says "open a circle", "ask the other sessions together", "get the other teams to decide this with us", "サークルミーティング", or "席を集めて聞いて". This session becomes the facilitator. It sends a skeleton (not a finished proposal), collects light views, revises, turns the skeleton into a proposal, and then lays out agreements, disagreements, and what nobody checked. It never rules or recommends, reports to the user after every stage, and waits for the user's OK before closing.
---

# session-circle: let running sessions think together

A circle is a discussion among Claude Code sessions that are already running on this machine. The session that opens it is the **facilitator**. The facilitator only sends, collects, lays out, and counts. **It does not rule, and it does not recommend.**

## 1. Before opening: three questions, asked for each session you want to invite

Ask these for **each** session separately. A session that fails any question is not invited; ask it one-to-one instead, or read the material yourself.

| Question | If "no" |
|---|---|
| Does this decision need something **only that session holds** (its own files, logs, settings)? | Ask one session, or read it yourself. |
| Do you want a different **view**, not just a "this would break" warning? | A warning is cheaper one-to-one. No circle needed. |
| Are you inviting **three sessions or fewer**? | Four or more: ask the user first, with the expected number of rounds. |

How to choose: prefer sessions that **do not share your assumptions** and that **can actually open and run the thing being discussed**. Invite the people who will use the result from the start; if you leave them out, write one line saying why. Include one session that has not been involved, so the same blind spot is not shared by everyone.

## 2. Five stages: skeleton first, flesh later

1. **Send the skeleton.** Not a finished proposal. Write: what must be decided, where the paths split, the **holes not yet filled**, and what already exists (who already does this job, what is already decided — with where you looked and how many you found, "0 found in X" if none). Write one line saying when this stage ends (for example: "if one round changes neither the splits nor the flow, go to the proposal"). Re-read it yourself first and remove numbers without a source and copying mistakes.
2. **Collect views.** Light: no format, as many times as needed. Ask every session the same first question: "Where did you look for anyone who already does this, or anything already decided, and how many did you find?" If someone is found, invite them.
3. **Revise the skeleton.** Show the list of changes, send version 2, and ask each session to point out anything you put in wrongly.
4. **Write the proposal.** Only after the skeleton is settled.
5. **One closing word from each session** on the proposal.

Rules for every stage:

- **Write every round's replies to a file in the same turn**, word for word, in the working folder (for example `circle_<id>_round<N>_<date>.md`). Messages between sessions live only in the receiving session's conversation; if that session closes, they are gone. Do not summarize — a summary turns "might change" into "will change".
- **Never write "no reply needed"** when you want an answer. Ask for one line even if there is nothing to change, so "read it and agree" can be told apart from "did not read it".
- **Everyone sends only to the facilitator.** Sessions do not message each other directly. The facilitator passes views on without names.
- **After each stage, report to the user before going on**, in the user's words: the original question, what this stage found or decided ("nothing" if nothing), why, what is left and who owns it, and what you need from the user.

## 3. Laying it out

Quote the sessions' words; keep your own summary separate. Show:

- **Agreements** — count by independent source, not by number of sessions (three sessions that read the same file are one source).
- **Disagreements** — do not say which side is right.
- **What nobody checked** — the next thing to measure. Write "none" if empty.
- **Where each session looked** for existing owners and decisions (one line each).

Do not add a recommendation: the facilitator is the only one who knows who said what.

## 4. Closing: wait for the user's OK

- Do not close when the layout is ready. Show it to the person who asked for the circle (usually the user), with the original question and whether it was answered (answered / partly / not), what is left and who owns it.
- While waiting, tell the sessions: "the circle is still open; please keep your session running."
- If the user pushes back, continue the same circle. If the user rejects the skeleton itself, go back to stage 1 rather than proposing your own answer on the spot.
- After the OK, send one closing message to the sessions, then tell the user: the original question, the answer (or that there is none), the reason, what is left, and what you need from them.
- Never write "solved". The teams and the user decide.
