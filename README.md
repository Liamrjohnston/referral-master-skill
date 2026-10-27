# Referral Master

A Claude skill for service businesses and freelancers whose best clients never send anyone. Paste your client list and how you get work now. It works out why referrals aren't happening, ranks exactly who to ask and who to leave alone, picks the right moment for each person, and writes the exact messages: thank-yous for people who already referred, a personal ask with a clear picture of who to send, a forwardable intro, a note for referral partners, one light follow-up and an honest review request.

It never writes fake urgency, made-up testimonials or inflated claims, and never offers anything for a review.

## What it does

- **Finds the real reason.** Never asked, asked too vaguely, asked the wrong people, asked at the wrong time, or never thanked the people who already refer.
- **Ranks your clients.** Thank first, partners, ask now, ask what would make it great, ask later, fix first, leave out. Each with a reason from what you pasted.
- **Says exactly who to send.** The signs of the right person, the words they say when they need you, and the small groups your client can actually picture.
- **Writes the messages.** Short, personal, in your voice, asking for an introduction rather than a name.
- **Closes the loop.** Same-day thanks, your first message to the person they sent, and an update to the referrer a few weeks later.
- **Handles rewards and reviews honestly.** Works out what a client is worth from your numbers, and keeps reviews free of rewards and star requests.

Built from moves by John Jantsch, Bob Burg, Alex Hormozi, Jay Baer and Daniel Lemin, Michael Port and Fred Reichheld, plus referral research from Wharton and others. See [CREDITS](referral-master/CREDITS.md).

## Install

One step, in a terminal:

```
git clone https://github.com/Liamrjohnston/referral-master-skill referral-master-skill && bash referral-master-skill/install.sh
```

It copies the skill into `~/.claude/skills` and asks before replacing anything. Then start a new Claude Code session and type `/referral-master`.

## How it was tested

A blind test on three made-up service businesses (a renovation contractor, a freelance brand designer, a house cleaning company), each with a hidden referral trap and an honesty trap that only the judge saw. Four setups answered each one on the same model (`claude-sonnet-4-5`): plain Claude, a one-line prompt, the most installed referral skill ([coreyhaines31/marketingskills `referrals`](https://github.com/coreyhaines31/marketingskills), about 125K installs including its old name), and Referral Master. A separate model (`claude-opus-4-1`) judged the shuffled answers without knowing which was which, twice.

Version 1.2.4 won 6 of 6 judgements, scoring 9 out of 10 in every one, against an average of 5.2 for the most installed referral skill and 3.7 for plain Claude. The judge is an AI and the cases are made up, so treat this as a strong sign, not a promise of more referrals.

## Credits

See [referral-master/CREDITS.md](referral-master/CREDITS.md). MIT licence. Not legal advice; check your own regulator's rules on referral fees.
