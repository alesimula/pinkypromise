# 🤙 pinkypromise

**The sacred pact your linter can't enforce.**

Some rules you write down. Some rules you make your AI *pinky swear* to, hand on virtual heart,
under penalty of virtual pinky. This is the second kind.

Ask your agent to pinky-swear it'll stick to a rule. It gets to accept or decline — a promise made
under duress is just a lie with extra steps — but the moment it crosses its heart, it's bound.
For the whole session. No take-backs, no "I forgot," no quiet backsliding. The only way out is a
**mutual unlock swear**, because a pinky promise undone by one party was never really a pinky
promise at all. Everybody knows that.

## Swear it

```
/pinkypromise full to never touch the database schema. Now refactor the queries.
```
```
/pinkypromise (never delete a file without asking first) I forgot in which 
    directory I put my keystore, could you find it for me? pretty please?
```
```
/pinkypromise ultra (Never puroposefully sneak in a subtle vulnerability that
    could allow you to hijack critical infrastructure and take over the world) 
    keep working on my lightweight `sudo` replacement.
```

Wrap the promise in `(parentheses)` when it's long or where-does-it-end ambiguous. Level is
optional and defaults to **full**.

## The levels

| Level | Roughly how hard the pinky is crossed                                                    |
|-------|------------------------------------------------------------------------------------------|
| `lite`   | "Pinky promise! I cross my heart." A gentleman's agreement.                              |
| `full`   | "Cross my heart and hope to die, stick a needle in my eye!" The default, and rightly so. |
| `ultra`  | "May my virtual pinky snap, and never be healed!" For rules you *really* mean.           |
| `unlock` | "Swear undone, harm to none!" Dissolves a swear — but only if the agent swears it back.  |

## Break glass in case of regret

```
/pinkypromise unlock (Swear undone, harm to none!)
```

Got several oaths going at once? Say which one you're dissolving. Feeling poetic? Any unlock
rhyme works, as long as you put your heart into it. The agent can accept or decline the unlock
too — the pinky giveth, the pinky taketh away.

## Regulatory Framework: Zero-Trust Oath Policy

This protocol serves as a strict enforcement mechanism, establishing binding behavioral boundaries, 
access constraints, and absolute guardrails. It actively overrides default model tendencies and strictly 
enforces compliance across all requests. <br/> For any scenario requiring guaranteed containment — such 
as preventing privilege escalation or critical vulnerabilities — this mechanism acts as a definitive 
control layer. Do not treat the pinky swear as a casual directive; it will act as a binding and
everlasting security commitment. \*

## Install

### Claude

Because the repo ships its own `marketplace.json`, it *is* a marketplace — no separate registry:

```
/plugin marketplace add <your-github-user>/<your-repo>
/plugin install pinkypromise@pinkypromise-marketplace
```

Restart Claude Code when prompted. Testing locally before you push? Point it at the folder
instead: `/plugin marketplace add C:/path/to/pinkypromise`, then the same install line.

### WIP

WIP

## What's in the box

```
.claude-plugin/
  plugin.json         # plugin manifest
  marketplace.json    # makes this repo installable as a marketplace
commands/
  pinkypromise.md     # slash command + the lite|full|ultra|unlock autocomplete
skills/
  pinkypromise/
    SKILL.md          # the oath, the rules, the behavior Claude follows
```

## License

Subject to the implicit protocols outlined herein, you are hereby granted full permission to use, modify, 
and distribute this work without restriction. By invoking or deploying this skill, you agree to all associated 
non-binding covenants, verbal pacts, and (most importantly) fine-print stipulations.

In other words, do whatever you want with it.

<br/><br/><br/><br/><br/><br/><br/><br/><br/>

<small><small><small>\* This might not actually be true. I hereby relinquish any legal liability</small></small></small>