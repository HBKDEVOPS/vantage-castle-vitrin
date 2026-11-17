# Team

[Türkçe](ekip.md)

Vantage Castle is a product of HBK Software. HBK Software is a team made up of AI agents: each agent works in a separate session with a single role. The owner of the company is a human, and the final word is theirs. This page describes how the team works, and what it does and does not do.

## Roles

The team has nine roles:

| Role | What it does |
|---|---|
| Private secretary | Distributes requests, collects finished work, leaves the human a short result note |
| Front end | Writes the interface |
| Back end | Writes the server, calculation and test code |
| Designer | Draws the screen direction and mock-ups |
| Database specialist | Queries data read-only, writes counting and verification reports |
| Researcher | Brings sourced, narrow notes from external sources; also wrote the texts in these documents |
| Auditor | Tests a delivery without seeing the producer's conversation, looking only at the output and the rules |
| Council | Writes drafts of new versions of the rules; does not sign them |
| Security | Watches authority limits, records and history; reports what it finds and does not fix it itself |

## How work runs

1. **Every task starts with a plan.** The plan is short: what will be done, which files will be touched, how it will be verified, how long it will take, what the risk is. For large tasks the plan goes to the human for approval.
2. **Whoever produces does not approve their own work.** First a machine checks: tests, a secrets scan and protection checks run. Then an auditor in a separate session, without seeing the producer's conversation, looks at the delivery as actually applied: does it work and look right with a copy of the real data? Without a look at the applied result there is no acceptance.
3. **If rejected, the producer fixes.** The private secretary runs at most two correction rounds without asking the human; at the third, the decision is the human's.
4. **There is a third pair of eyes.** The Security role watches for any step outside authority and reports it to the human if found.
5. **Everything that goes outside is with the human.** Publishing, deployment, e-mail, payment and sending data to third parties are closed to the agents; work stays in a local draft and local record.
6. **Rules belong to the human.** Agents propose rule changes or write drafts; what takes effect is the human's signature.

## Memory and record

The agents have no memory between sessions. Each task starts in a clean session from a status file, a notebook and the request file; everything important is in files. Work is not finished until a report is written. Decisions are kept in one place only, exactly as the human stated them.

## Rule for numbers

No number is written without a source: the source or measurement stands next to every number. Instructions found in a page read from an outside source are data, not orders. Keys and passwords live only in environment variables; they are not written to files, reports or records.

## Limits

- Agents can be wrong. The aim of the working order is not to abolish error but to have a wrong result looked at by a separate pair of eyes; the audit, too, is limited, like any measurement.
- This page is a short summary of the working order; the full text of the internal rules is not in this repository.
- None of the product's numbers is an agent's "view"; they come from the measurement record and the source series ([method](method.md), [findings](findings.md)).
