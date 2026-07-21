# pinkypromise

A Claude Code plugin. Ask Claude to pinky-swear it will stick to a rule. It may accept or
decline — but once it swears, it's bound for the rest of the session, unlockable only by a
mutual unlock swear.

## Install

```
/plugin marketplace add <your-github-user>/<your-repo>
/plugin install pinkypromise@pinkypromise-marketplace
```

Then restart Claude Code when prompted.

## Use

```
/pinkypromise full to never touch the database schema. Now refactor the queries.
/pinkypromise (never delete files without asking) go clean up the build dir.
/pinkypromise unlock (Swear undone, harm to none!)
```

Level is optional and defaults to **full**. Levels: `lite`, `full`, `ultra`, `unlock`.

## Layout

```
.claude-plugin/
  plugin.json         # plugin manifest
  marketplace.json    # makes this repo installable as a marketplace
commands/
  pinkypromise.md     # slash command + argument-hint autocomplete
skills/
  pinkypromise/
    SKILL.md          # the behavior Claude follows
```
