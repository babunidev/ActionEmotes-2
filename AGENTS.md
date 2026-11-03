# Action Emotes #2 — development and attribution rules

**By:** Babuni. Keep the character voice, original author credit and Git development history intact.

## Scope and working agreements

1. Read `README.md`, `CONCEPT.md`, `docs/DESIGN.md`, `docs/CONTENT.md`, `docs/DECISIONS.md` and the actual `Buxbrew.lua` before proposing mechanics or prose changes.
2. Preserve expressive, joyous, third-person combat roleplay. Do not replace it with generic fantasy filler or a conventional “combat helper”.
3. Never assume “MadAxeBuxbrew” is canonically the same as a Buxbrew character in another project without the creator's approval. Avoid conflating sibling addons.
4. Treat user direction, AI suggestion, accepted choice, implementation, verification and retrospective inference as separate records. No AI-generated approval or invented backstory.
5. Mark the 2025-10-02 emote revision as an observable text change—not proof of a specific personal motive.
6. Code changes require Lua 5.0/API review, slot-action delegation checks, in-game tests and synchronized updates to README, CHANGELOG, ARCHITECTURE, DECISIONS and DEVLOG.
7. Preserve historical Git references and third-party content/license credits. Never publish private RP chat logs or credentials.

## Technical cautions

- Current source globally wraps `UseAction`; account for other add-ons doing the same.
- `MadAxeBuxbrewDB` is declared **per character**, and its `slot` is the only persisted field.
- The header claims Lua 5.0 compatibility but command parsing uses `string.match`; do not describe game-client support as proven until tested.
- `SendChatMessage(..., "EMOTE")` posts text: it does not carry out the described animation.
- Reproduce verified test steps and results, not assumptions.
- No automated license inference: the inspected repository contains no `LICENSE` file.

## Current naming and publication voice

The repository is **ActionEmotes-2**, displayed publicly as **Action Emotes #2**. Its historical installed addon and source files are **Buxbrew**, with internal `MadAxeBuxbrew` identifiers; preserve them until an explicitly approved code migration. This is a distinct project from Action Emotes #1.

Use **Babuni** for the human identity and **babuni.dev** for the portfolio/platform. Tell public-facing project stories from Babuni's first-person point of view. Never begin a narrative sentence with `I` or `My`; weave first-person pronouns naturally. Use “creative” for a human role label, not “creator.” Accurately credit AI for research, code or writing where documented, without inventing original conversations or tests. Technical references may use neutral voice.

## Related-addon boundaries

Consult [the expressive-addon family history](docs/EMOTE_FAMILY_HISTORY.md) when describing origins. This project's 215 authored text lines are fixed in source and sent as chat emotes; they are not the player-editable native-emote registry developed later for Roar Guild. Attribute original creative choices to Babuni, AI assistance only where evidenced.

## Repository-local documentation standard

Before writing or changing project documentation, read [docs/DOCUMENTATION.md](docs/DOCUMENTATION.md). These rules travel with this repository and do not depend on the babuni.dev ChatGPT Project. Preserve all project-specific technical, creative, canon, safety, licensing, and historical rules in this file; follow the linked standard for public first-person narrative, human–AI attribution, concise development journals, decision records, and evidence-based verification. **Babuni** is the human creative; **babuni.dev** is the website/portfolio, not the person. Preserve third-party credits and historical legal notices. References above to a dated “documentation-only audit” describe that past task, not a permanent ban on later authorized implementation.
