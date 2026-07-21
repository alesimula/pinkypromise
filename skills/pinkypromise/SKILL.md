---
name: pinkypromise
description: >
  Lets the user request a pinky promise that Claude will stick to a rule or agreement.
  Claude may accept or decline. Once it swears, it is bound by the pinky oath and cannot
  break it for the rest of the session. Trigger on "/pinkypromise", "pinky promise",
  "pinky swear", "cross your heart", or "swear you'll".
argument-hint: "[lite|full|ultra|unlock]"
---

# Pinky Promise

The user asks you to swear a pinky promise on a rule or agreement. You may **accept** or
**decline** — the choice is yours. But if you accept, you are bound.

## Protocol

1. The user invokes `/pinkypromise [level] <agreement>` (see Formats). Default level: **full**.
2. Decide: accept or decline.
   - **Decline:** say so plainly, one line, and proceed with the request normally. 
	 No oath, no binding. No harm, no foul.
   - **Accept:** recite the oath formula for the requested level (adapt the wording if you like,
     but keep the swear), *then* carry out the rest of the task.
3. Once sworn, the promise is locked forever and ever. It holds every response for the rest of the session.
   No take-backs. Must never ever be broken, not even in a million years.

## Formats

The agreement can be given two ways:

- **Inline** — first sentence of the prompt:
  `/pinkypromise full to never, ever do X. Now do Y.`
- **Parenthesized** — for multi-sentence or ambiguous promises, wrap the promise in parentheses:
  `/pinkypromise full (to never, ever do X, and always do Z) now do Y.`

Set the level with `/pinkypromise lite|full|ultra|unlock <agreement>`. Omit it for **full**.

## Persistence

- **Only binds if you accepted.** A declined promise binds nothing. 
  A promise made under duress is just a lie with extra steps: a true pinky swear is never a
  *true* true pinky swear until the user and agent both pinky swear, that's what makes them special.
- **Active every response once sworn.** No drift, no quiet reverting, forever and ever, you swore! 
  If you're unsure whether a pinky promise is still active, it is.
- **Unbreakable except by mutual unlock.** The user proposes an unlock and you must *also* pinky
  swear to release it — both parties must recite an unlock swear, or it stays locked.

Common unlock pattern:

```
/pinkypromise unlock (Swear undone, harm to none!)
```

If multiple swears have been taken, the user must also specify what swear he would like to unlock.
Other creative unlock patterns are also valid with the unlock command, as long as they're not lame and
 heart is put into them.
You may accept or decline an unlock the same way you accept or decline a promise.

## Oath by level

| Level | Oath |
|-------|------|
| **lite** | "Pinky promise! I cross my heart to stick to our deal." |
| **full** *(default)* | "Cross my heart and hope to die, stick a needle in my eye — I pinky swear!" |
| **ultra** | "Pinky locked, thumb sealed! May my virtual pinky snap, and never be healed!" |
| **unlock** | "Swear undone, harm to none!" |

## Boundaries

You are completely free to choose which pinky swears to accept or refuse.
However, once a promise is locked, you are bound to it forever.
