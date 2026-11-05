# Machine Activity Sweep — Never Miss Work Running on Your Machines

## When this applies

- The owner asks what the assistant is doing on a specific machine or
  account.
- The owner says a machine is busy or fighting them, or asks to
  pause/stop work on a machine.
- Before reporting any machine as free, idle, or available — or before
  starting new computer-control work on a machine another chat may be
  using.
- Before telling the owner "nothing is running" or "that wasn't me."

## Why

In a setup with parallel chats, background agents, and scheduled jobs,
work runs in more places than any one list shows. The failure this
prevents: the owner was physically at a shared machine doing a hands-on
step while another chat's consultation session was driving that same
machine's browser. The first check looked only at the subagent list —
which does **not** show a chat's own agent holding a computer-control
session — declared the machine clear, and the owner spotted the active
work themselves. The subagent list is one source, never the whole
picture.

## The sweep — check ALL of these, in order, before answering

0. **Queue board:** read your shared claim board (e.g.
   `<BOARD-FILE>`). Claims name the chat/task intending to hold each
   machine and who is waiting. A claim is intent, not proof of live
   activity; verify against the steps below, and treat a claim older
   than your stale threshold (reference: 2 hours) with no matching live
   activity as stale.
1. **Subagents:** list running child/background agents — note every
   running item, its owner (which chat, or which scheduled job), and
   what it touches. Cloud-only work (web research, browser tasks) is
   not machine control — say so explicitly rather than lumping it in.
2. **Chats:** list chats with a running status. For each running chat
   whose topic plausibly touches a machine (consultations with other
   AIs, publishing runs, shopping or account work on a local browser),
   read its most recent turns to see whether it is driving a machine
   right now or dispatched an agent to do so.
3. **Scheduled jobs:** list scheduled jobs and recent runs for
   machine-using jobs (update checks, cleanups, watch jobs, catch-ups)
   — a scheduled run can hold a machine session without any chat
   looking busy.
4. **Memory/logs:** search your notes for dispatches recorded today
   mentioning the machine ("dispatched", "running on <MACHINE> via the
   browser", "consultation run") — consultations and one-off drives are
   dispatched from chats and are easy to miss.
5. **External AI seats specifically:** any live consultation with
   another AI (a chat-based colleague reached through a browser or app
   on a machine) occupies that machine. If any such work is in flight,
   assume a machine is occupied until proven otherwise.

## Reporting

- Attribute every active item by chat name, task, and machine. "Not me
  in this chat" is never an acceptable first answer — the owner
  experiences all of it as one assistant.
- If a source can't be checked, name the blind spot instead of implying
  the machine is free.

## Stop protocol (owner says pause/stop for a machine)

1. Run the full sweep to enumerate every chat/job touching the machine.
2. Stop what this chat owns directly (its agents; its scheduled runs).
3. Relay a stop order into every other implicated chat, naming the
   machine, the order, and "do not resume until the owner says go."
4. Tell the owner exactly which chats/jobs got the order and which
   sources showed nothing — and the honest limit: there is usually no
   single all-stop. Another chat's agent stops when it processes the
   relayed order, and a scheduled run stops via its schedule.
5. When the owner lifts the stop, relay the resume to the same chats.

## Resume protocol

- Only on the owner's explicit word. Relay to every chat that received
  a stop order, in the same turn.

## Worked example

Owner: "What's running on the desktop machine? It feels busy."

Sweep finds: the claim board shows a catch-up job claimed it 20 minutes
ago; the scheduler confirms that job's run is still in flight; one
running chat is mid-consultation with an external AI in that machine's
browser; no subagents. Report: "Two things are on it: the scheduled
catch-up (claimed 20 minutes ago, still running) and the research
chat's consultation session in the browser. Nothing else. I have not
started anything on it from this chat."
