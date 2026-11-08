# Florian Przybylak

OT/IT architect. I build small infrastructure tools that answer one technical
question each, with a demo you can run yourself and limits stated next to the
result. Industrial networks are where most of them come from; none of them
needs an industrial project to be useful.

## Developer tools

| Tool | The question it answers | Try it |
| --- | --- | --- |
| [TrailMQ](https://github.com/RainerGewalt/TrailMQ) | Why was my MQTT access denied? A self-hosted broker that controls access and records the check that refused a publish or subscribe. | `./trailmq try`, then the [reproducible proof](https://github.com/RainerGewalt/TrailMQ/blob/master/docs/why-was-my-mqtt-access-denied.md) against a secured Mosquitto |
| [Trail Evidence](https://github.com/RainerGewalt/trail-evidence) | Is this event journal intact? One JSON record format with a hash chain, and verifiers in Go, Python and the browser that agree. | [Verify in the browser](https://rainergewalt.github.io/trail-evidence/), nothing is uploaded |
| [TrailSource](https://github.com/RainerGewalt/trailsource) | What changed in my OPC UA data source? A read-only adapter that records every observation, address-space change, gap and restart as a verifiable record. | `make scenario-server-restart` against the bundled simulator |
| [TrailTransfer](https://github.com/RainerGewalt/trailtransfer) | Which file transfers ran at the edge, and with what result? Policy-restricted rclone jobs over MQTT, every outcome in a verifiable journal. | `make quickstart` |

Trail Evidence, TrailSource and TrailTransfer are Apache 2.0. TrailMQ is a
free, non-production evaluation under its own licence; how developers may
use it beyond evaluation is an open question for the project. Each tool works
on its own; none of them requires the others.

## Personal software

| Tool | What it is |
| --- | --- |
| [Plainlane](https://github.com/RainerGewalt/plainlane) | A small self-hosted task board for everyday projects: tasks, steps, files, notes and emails in one SQLite file. MIT. |
| [Track Forge](https://github.com/RainerGewalt/track-forge) | A track studio for [Strudel](https://strudel.cc): see the arrangement lanes of your patterns, audition edits before saving, listen on your phone over the LAN. AGPL. |

## Working with these projects

Every repository has an **Evaluation report** issue form. A first run that
failed is as useful as one that worked. Support is best effort: issues are
read and answered, without a guaranteed response time, SLA or paid support.
Security reports go through each repository's private vulnerability form,
never through a public issue.

I write about what happens after industrial systems are connected: trust,
responsibility, traceability and control. [LinkedIn](https://www.linkedin.com/in/florian-p-6a27ab1b8/) · [trailmq.com](https://trailmq.com)
