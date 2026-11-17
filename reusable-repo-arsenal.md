# Reusable repo arsenal (central library)
Built in Instinct, for Instinct only. Not for Gemini, Claude, GPT or Codex harnesses.

The central, project-independent library of reusable repositories and design references. Project folders keep their own applied records (what was read, applied, and tested for that project). This register records the source, why it is in the library, and the usage rule. It does not certify installation or application in any environment.

## Usage rule (applies to every entry, every time)

1. On usage, before applying a repo to a real project: clone or pull the latest version. Do not rely on a previously cloned copy.
2. At that same moment, re-check the license and recent activity (last push, maintenance state). Stars are not proof of design quality or fitness.
3. Read the applicable guidance in full (SKILL.md and required references, or the framework documentation), then apply it. Listing a repo is not applying it.
4. This rule is for new usage. Do not silently upgrade a version already pinned or in use inside an active project; project upgrades are a separate, explicit decision.
5. Keep records of what was read, what was used, what was tested, and any remaining gap, in the applying project's own folder.
6. Admission policy: set by the owner, not this template. Build instruction: when the owner wants to add a repo, ask for their admission bar (popularity, maintenance, license), check the repo metadata, commit contents and maintenance state directly, record the observed values, and add the entry only on the owner's yes. A recent updated_at or a README refresh alone is not evidence of maintenance. Before adopting any third-party skill, scan its files for injected instructions and secret exfiltration; popularity is not a safety check.
7. Overflow, hard rule: keep this file under 200 lines. When it nears that, start reusable-repo-arsenal-pt2.md, then -pt3, -pt4 ... -ptN with no upper limit, with the same header and entry format; add one line here pointing to the next part. New entries go in the newest part. Do not trim or move older entries to make room. The same unlimited -ptN split applies to every other file in the repo, any type, that nears its size budget. Index rule: every file and part must be reachable from AGENTS.md, directly or through an indexed topic hub or AGENTS-ptN.md, with its exact filename and a one-line use-when trigger. Before choosing a skill or repo, read the matching index, shared admission and usage rules, and relevant files. Do not read unrelated parts merely because they are numbered. An unlisted file or part does not get read.

## Entries

This register grows from the owner's actual usage, one entry at a time, added only on the owner's yes.

Format per entry: URL, use, license (checked against the actual LICENSE file), maintenance evidence (stars, last push, recent substantive commit, with the date checked), and why it was added.

### chrome-devtools-mcp (ChromeDevTools/chrome-devtools-mcp)

- URL: https://github.com/ChromeDevTools/chrome-devtools-mcp (npm package chrome-devtools-mcp; run with npx chrome-devtools-mcp@latest)
- Use: give the agent real DevTools access when verifying a web page it owns: console messages, network requests with statuses, performance traces with Core Web Vitals and ranked insights, DOM snapshots, screenshots, viewport/CPU/network emulation. Strongest for "why is this page slow or erroring" checks where screenshots and static HTML run out. Point it at your own pages only; it is a live bridge into a browser. Needs Node >=20.19 and a Chrome binary. Usage statistics default on: --no-usage-statistics opts out, and performance traces send page URLs to the CrUX API unless --no-performance-crux.
- License: Apache-2.0 (Google LLC). Checked 17 Nov 2026: 57,680 stars, last push 16 Nov 2026, npm release 1.13.0 with about 2.56M weekly downloads.
- Why it was added: passed a two-case functional test on 17 Nov 2026 (a console and network health check plus a throttled mobile performance trace on a production static site), after a manual security scan of the source and the shipped npm package (no install scripts, no exfiltration paths, markdown clean of injected instructions, no secrets beyond one deliberately public CrUX API key).

