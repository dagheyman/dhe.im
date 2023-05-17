---
title: "Abbreviations for business continuity"
date: 2023-05-17
draft: false
---

When things go wrong, how long does it take you to be back on track? Is there a plan in place?
This is what _business continuity planning_, _disaster recovery_ and, in some sense, even _incident response_ are all about. Let's learn a few abbreviations in this area. These are all part of the [Security+](https://dhe.im/posts/security-plus/) material (surprise!), but I think they represent interesting questions to ask as anyone responsible for the reliability or security of a production system.

| Abbreviation  | Description |
| -------- | -------- |
| RTO - Recovery Time Objective | The recovery time objective defines the maximum tolerable time it can take to restore a system after an outage. |
| RPO - Recovery Point Objective | A recovery point objective defines how much data loss is acceptable, by setting a point in time.
| MTBF - Mean time between failures | This is a measurement of a systems reliability, usually in hours. It's defined as the average time between failures.
| MTTR - Mean time to repair | The mean time to repair refers to how long it takes, on average, to restore a system after a failure.

Re-phrasing all this as questions to ask about our resilience we get:

- How long can we survive without this system? (RTO)
- How often do we need to run backups? (RPO)
- How often does this system go down? (MTBF)
- How long does it take us to fix it? (MTTR)

I hope you have at least discussed these, so that when a disaster happens, recovery can be as smooth as possible.
