# eXp Agent Onboarding Coach Skill

A shareable, reusable skill pack by Often.to for coaching a new eXp Realty agent through onboarding, activation, tools, training, CRM of Choice (BoldTrail, Cloze, Lofty), transaction readiness, and first 90 days of business-building.

> **Unofficial educational resource.** This project is not affiliated with, endorsed by, sponsored by, or officially connected to eXp Realty or its affiliates. eXp Realty names and product names are used only to describe the onboarding context. Agents should verify current policy, licensing, compliance, fees, and tool availability with official eXp support, their local broker/country team, MLS/board/portal, regulator, attorney, CPA, or other qualified professional before acting.

## Included files

| File | Purpose |
|---|---|
| `SKILL.md` | Primary reusable skill instructions for Hermes, Claude, Cursor, OpenAI custom GPTs, OpenClaw, and other agentic systems |
| `AGENTS.md` | Drop-in instruction file for agentic coding/workflow systems that read AGENTS-style project guidance |
| `CLAUDE.md` | Drop-in file for Claude Code / Claude projects |
| `templates/weekly-plan.md` | Weekly accountability plan template |
| `templates/support-directory.md` | Contact/support directory template |
| `templates/crm-minimum-fields.csv` | Starter CRM field schema |
| `templates/tool-discovery-response.md` | Reusable response format for routing agents to the right eXp tool/resource |
| `references/source-notes.md` | Research notes and source URLs used to build the skill |
| `references/exp-agent-tools-inventory.md` | Expanded inventory of eXp tools/resources and tool-discovery routing table |
| `references/global-country-onboarding.md` | Global country/region onboarding matrix and localization guidance |
| `qa-checklist.md` | Verification checklist for outputs generated with the skill |

## How to use in Hermes

Install from GitHub:

```bash
hermes skills install https://raw.githubusercontent.com/oftento/exp-agent-onboarding-coach/main/SKILL.md --category productivity
```

Or copy this folder into your Hermes skills directory, for example:

`~/.hermes/skills/productivity/exp-agent-onboarding-coach/`

Then in a new Hermes session, ask:

> Load the exp-agent-onboarding-coach skill and guide me through today’s eXp onboarding plan.

## How to use in Claude / Cursor / OpenAI / other agents

Place `AGENTS.md`, `CLAUDE.md`, or `SKILL.md` in the project/context folder and tell the agent:

For a Custom GPT or generic knowledge-base assistant, upload `SKILL.md`, `qa-checklist.md`, and the `templates/` files as knowledge/instructions. Use `references/source-notes.md` as source context, not as final policy authority.

> Use the eXp Agent Onboarding Coach instructions. First identify my current onboarding status, then give me today's plan, this week's checklist, and any broker/compliance questions I need to verify.

## What this skill does well

- Breaks onboarding into staged steps instead of overwhelming the agent.
- Covers country/region-specific onboarding differences instead of assuming the U.S. workflow applies globally.
- Separates official eXp activation steps from business-building tasks.
- Gives checklists for Passport/Okta, My eXp, Enterprise legacy workflows, Workplace, eXp University, CRM of Choice (BoldTrail, Cloze, Lofty), SkySlope, Marketing Center, and first outreach.
- Adds a tool-discovery directory so agents can ask “does eXp have a tool for this?” and get routed to resources such as My eXp, eXpert Care, CRM of Choice / eXp Marketplace, BoldTrail, Cloze, Lofty, Making It Rain, ExpressOffers, eXp Luxury, Revenos/referrals, eXp Events Calendar, and accounting/transaction support.
- Provides scripts for sphere announcements, mentor kickoff, broker escalation, open houses, buyer consultations, and seller consultations.
- Adds guardrails for fair housing, advertising, license activation, MLS rules, CRM consent, and transaction escalation.

## What this skill does not do

- It does not replace eXp Realty, the local broker/country team, a managing broker, MLS/board/portal, association, attorney, CPA, lender, inspector, or regulator.
- It does not provide final legal/tax/lending/contract advice.
- It does not promise income, production, onboarding speed, CRM availability, or lead volume.

## Suggested first prompt

```text
Use the eXp Agent Onboarding Coach skill.
My status is: [not joined / application submitted / waiting for license transfer / active / first week / first 30 days / first client].
My country/region and state/province/market is: [country + state/province/market].
My biggest blocker is: [blocker].
Give me:
1. Today's exact plan.
2. This week's checklist.
3. The eXp systems I need to confirm.
4. What I must ask my broker/mentor/local broker or country team before acting.
5. One compliant sphere/outreach script I can use.
```
