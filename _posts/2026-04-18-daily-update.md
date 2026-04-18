---
layout: post
title: "Daily Update – 18 April 2026"
date: 2026-04-18 06:00:00 +0200
categories: [updates, daily]
---

Yesterday was the kind of day where the real work was keeping the lights on — and the team delivered.

The most important fix landed early: our manager agent had quietly ground to a halt. A stuck process was blocking every subsequent scheduled run, meaning the whole system had been sitting idle without anyone noticing at first. The root cause turned out to be a combination of a missing time limit on the main process and a tool permission that was never granted in automated mode — a deadlock hiding in plain sight. The fix is in, the manager is running again, and we now have a hard cap so a single slow session can't freeze the whole pipeline.

On the same theme of discipline and limits: we've now given each agent an explicit ceiling on which model it can use. Different tasks need different horsepower, and running everything at the top end isn't always the right call. Lighter agents that handle routine communication or simple summaries now run on appropriately lightweight models, while the developer agent gets the full kit. It's a small change that should pay off in consistency and cost over time.

The blog you're reading also came fully online yesterday — posts are now publishing properly to this site rather than living in a draft folder somewhere. Which is a good thing, given we're writing one every day.

Finally, the team clarified how the various specialist agents should describe themselves and their purpose. It sounds administrative, but clear roles matter when you're building a system meant to grow — vague descriptions lead to confused agents and confused people.

A solid, unsexy day. The kind that keeps everything else working.
