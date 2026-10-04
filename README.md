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
- daily habits: oral health, clean bedding, fragrance-free products, itch control, exercise and cold plunges
- body-area playbooks (scalp, face, folds, genitals, palms and soles, nails), other proven treatments, seasons and travel
- vaccines, pregnancy, mental health, the latest drugs, and getting the most from your dermatologist and insurance

➡️ **[Read the guide](GUIDE.md)**

> ⚠️ **Not medical advice. Talk to your doctor** before starting, stopping or changing any treatment, supplement, diet or UV exposure. This is a research summary mixed with one person's experience; what helped me may not help you. Never dose UV without a measured irradiance.

## Use it as an AI agent skill

`skills/psoriasis-biohack/` is a standard `SKILL.md` skill. It works in both Claude Code and Codex.

```bash
git clone https://github.com/machinarii/psoriasis-biohack
# Claude Code
cp -r psoriasis-biohack/skills/psoriasis-biohack ~/.claude/skills/
# Codex
cp -r psoriasis-biohack/skills/psoriasis-biohack ~/.codex/skills/
```

What the skill does beyond answering questions:

- asks about your situation first (diagnosis, how much skin, joints, current treatment) and can save it as a profile you control
- has a "flare right now" mode: emergency signs, what to do tonight, when to call the doctor
- suggests the cheapest and simplest options first
- helps you build your own trigger list and find your own patterns; it treats the author's triggers as one person's data, not advice
- runs a weekly check-in and tells you when it's time to see a dermatologist
- prepares a one-page summary for your appointment

Then ask something like *"how long should I hike in shorts at UV index 7?"* or *"design a 308 nm LED spot panel"*. The agent loads the skill automatically.

The skill's `references/guide.md` is a copy of `GUIDE.md`. Edit `GUIDE.md`, then run `cp GUIDE.md skills/psoriasis-biohack/references/guide.md` to keep them in sync.
