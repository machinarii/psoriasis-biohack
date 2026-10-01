# Psoriasis Biohack

This guide comes from my own experience and research. I've lived with psoriasis since I was a child, and it collects what I've tried, what I've learned the hard way, and what the research actually supports.

It is an evidence-graded guide to managing psoriasis (with notes on eczema and oozing flares). It covers:

- narrowband UVB phototherapy and sun exposure while hiking
- red, near-infrared and blue light
- a DIY 311 nm lamp / 308 nm SMT LED phototherapy build
- topicals, including correct clobetasol use
- diet, dairy/whey triggers and dairy-free protein
- supplements, including histamine- and salicylate-lowering options, and supplements and foods with immune activation risk
- n-of-1 self-experiments

➡️ **[Read the guide](GUIDE.md)**

> Research summary, not medical advice. Confirm prescription use and UV dosing with a dermatologist. Never dose UV without a measured irradiance.

## Use it as an AI agent skill

`skills/psoriasis-biohack/` is a standard `SKILL.md` skill. It works in both Claude Code and Codex.

```bash
git clone https://github.com/machinarii/psoriasis-biohack
# Claude Code
cp -r psoriasis-biohack/skills/psoriasis-biohack ~/.claude/skills/
# Codex
cp -r psoriasis-biohack/skills/psoriasis-biohack ~/.codex/skills/
```

Then ask something like *"how long should I hike in shorts at UV index 7?"* or *"design a 308 nm LED spot panel"*. The agent loads the skill automatically.

The skill's `references/guide.md` is a copy of `GUIDE.md`. Edit `GUIDE.md`, then run `cp GUIDE.md skills/psoriasis-biohack/references/guide.md` to keep them in sync.
