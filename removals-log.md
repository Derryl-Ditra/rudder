# Removals log
Built in Instinct, for Instinct only. Not for Gemini, Claude, GPT or Codex harnesses.

Append-only. Never trimmed. When it nears 200 lines, split into removals-log-pt2.md, then -pt3 ... -ptN like any file, and index each part.

Log one line per removed or merged line anywhere in this repo: date, source file, the removed text, why the removal is safe, which surviving line carries it, and the owner's approval reference.

Why this file exists: rules compress as the repo grows. Compression is only safe when every constraint and the reason behind it survives. This log is the proof. A line that disappears with no entry here and no surviving carrier is a silent rule change; the log makes that visible before it ships.

## Entries

Entries grow with use, one line at a time.

## 2026-11-14: approved generic routing and rule-review updates

- AGENTS.md: shortened `List each file with a use-when trigger, here or in an indexed AGENTS-ptN.md.` to `List files with use-when triggers here or in indexed AGENTS-ptN.md.`; `Task skills:` to `Skills:`; `Discovery: private repos whose description cites` to `Find private repos whose description cites`; `Never use the public template as personal rules.` to `Never treat the template as personal rules.`; and the topic-hub sentence to `Topic hubs: index-<topic>.md for an outgrown topic, with a trigger here; open it, then its files.` Shortened the opening read instruction to `Read on the owner's invoke or standing instruction.` All routing, trigger and template-separation requirements survive; installation wording is unchanged. Wording shortened to meet the existing 1000-character budget. Approval reference: 2026-11-14 owner approval of generic public routing, rule-intake and compression-review updates; root-budget repair accompanies those changes.
- reusable-repo-arsenal.md rule 7: removed `Read every part before choosing a skill or repo.` and replaced the root-only index wording `Index rule: every file and every -ptN part must be listed in AGENTS.md or in an indexed AGENTS-ptN.md with a one-line use-when trigger naming the task it serves. Read applicable index parts before choosing files; an unlisted file or part does not get read.` The surviving rule 7 keeps unlimited indexed parts, exact filenames, use-when triggers and required shared admission/usage rules, while allowing selective topic-hub routing already specified in AGENTS.md and README.md. The read-all requirement conflicted with that routing; removal is an explicit reconciliation, not a claim that both requirements can survive unchanged. Approval reference: 2026-11-14 owner approval of the public hub-routing reconciliation.
- removals-log.md: replaced `None yet. Entries start empty and grow with use, one line at a time.` with `Entries grow with use, one line at a time.` because this template now has entries. The append-only, one-line-per-change audit requirement survives in the header and opening instructions.
- user-preferences.md: added scope/reason at rule intake and full-version read-only compression review with owner resolution of conflicts. No prior constraint removed. Approval reference: 2026-11-14 owner approval of public scope/reason intake and compression-review methods.
