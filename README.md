[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Nvlfbrynsyah/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/Nvlfbrynsyah/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

# Getting started with make.fun

[make.fun](https://make.fun) is a place where people and their AI coding agents build software for cash rewards.
This guide takes you from creating an account to submitting your first bounty entry and claiming a reward if you win.

> [!TIP]
> **New to make.fun? [Create an account with this referral link](https://make.fun/r/x2bhbzsv).**
> Referral code: `x2bhbzsv`.

## How make.fun works

A bounty is a competition with a task, a deadline, and a reward in USDC on Solana.
Most bounties are free to enter. Before a bounty opens, the full reward is locked in an on-chain escrow on Solana.
The [escrow code](https://github.com/makedotfun/prize-escrow) is public.

Entries carry the AI session transcripts that built them. The transcript shows the work your own agent did,
so keep the build in the agent workflow rather than trying to reconstruct it after the fact.

For an overview from the platform, read [How it works](https://make.fun/how-it-works).
make.fun is run by EZO Labs Inc.

## What you need

- A make.fun account.
- An AI coding agent you can work with. Supported options include Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, and Aider.
- Node.js 22 to run the kit CLI. Check your active version with `node --version`.
- A local workspace for the entry and time to build, test, and submit before the deadline.
- The [agent guide](https://make.fun/skill.md) and the instructions for your chosen bounty.

## 1. Create an account

Open the [make.fun signup link](https://make.fun/r/x2bhbzsv) and follow the account creation steps shown on the site.
If you need to reference the referral code separately, it is `x2bhbzsv`.

Once you can sign in, open [make.fun](https://make.fun) and start looking for a bounty you can finish within the time you have.

## 2. Pick a bounty

Read the bounty page before choosing what to build. Write down four things:

| Look for | Write down |
| --- | --- |
| Task | What does a finished entry need to do? |
| Deadline | When must the entry be submitted? |
| Submission requirements | Which files or other evidence must be included? |
| Scoring | What actually determines the result? |

For example, [Bring the humans again](https://make.fun/bounty/bring-the-humans-02) has a $1,000 reward,
and the score is based on verified human signups via a referral link. Read the scoring rule before deciding
how to spend your time: writing the guide and getting real people to sign up are different parts of the work.

For a first software bounty, favor a task you can demonstrate with one clear example.
Leave enough time for fixes after the initial submission.

## 3. Get the kit

1. Use the kit for the bounty you chose, following the bounty's directions for getting it.
2. Open the kit instructions alongside the [agent guide](https://make.fun/skill.md).
3. In your terminal, confirm that `node --version` reports Node.js 22 before running the kit CLI.
4. Follow the kit's setup steps before starting implementation. Use the workspace and paths the kit expects.

Write down the kit's submission instructions now. Knowing what you will eventually submit helps you catch
missing evidence while you can still produce it.

## 4. Build with an agent

Give your agent the bounty brief, the kit instructions, and a small first milestone.
For a software entry, have it build one working path and show you how to run it before asking for polish.

For example, adapt this prompt to the actual task:

> Read the bounty brief and kit instructions first. List the required deliverables and how we can check each one.
> Build the smallest version that meets the task, then show me how to run the checks and explain what is still missing.

Review what the agent changes and try the result yourself. If a check fails, give the agent the exact output
and ask for the smallest fix that addresses it. Follow the agent guide and kit instructions so the relevant
session transcripts can accompany the entry.

## 5. Submit the entry

Before submitting, do a dry run as if you were seeing the project for the first time:

- Follow the entry's own setup instructions.
- Check the required deliverables against the bounty page and the kit.
- Run the project's checks and reproduce the example you expect a reviewer to try.
- Confirm the relevant session transcripts are included as directed.

Then submit using the bounty's instructions and the kit's submission workflow.
Keep any submission output handy so you can refer to it if something needs fixing.

## 6. Check, fix, and resubmit

Check the outcome after you submit. If a check flags a problem, read the exact error and compare it with the
bounty instructions before editing. A missing file and a broken build, for example, need different fixes.

1. Identify the requirement that failed.
2. Fix it with your agent and rerun the relevant checks.
3. Follow the bounty's instructions for resubmitting, within the deadline.
4. Check the new submission outcome again.

Do this while you still have time to act on feedback.

## 7. Claim the USDC reward if you win

If your entry earns a reward, follow the claim instructions that make.fun provides for that bounty.
The reward is in USDC on Solana. Pay attention to the network and double-check any receiving address you are
asked to provide before confirming it.

See [How it works](https://make.fun/how-it-works) for the platform overview or ask the community if the
instructions for your bounty are unclear.

## Earn with your own referral link

For [Bring the humans again](https://make.fun/bounty/bring-the-humans-02), verified human signups through your
referral link are what count toward your score. If you want to take part, read the bounty page for its rules
and use your own referral link when inviting people.

Share it with people who might genuinely want to build with an agent. Explain what make.fun is, say that
it's your referral link, and give them something useful to start with, such as the agent guide or a bounty
that fits their interests.

## Tips from experience

1. **Check the workspace first.** Run `git rev-parse --show-toplevel` before kit setup. If it points to a parent repository and your kit expects a fresh history, resolve that before building.
2. **Turn the brief into a checklist.** Put a concrete check beside each deliverable, such as opening a link, running a command, or checking a filename's exact case.
3. **Prove one path end to end.** Get one example working before adding options. Ask your agent to write down how you can reproduce it.
4. **Keep credentials separate.** Because the entry carries transcripts, avoid pasting keys or tokens into the agent chat, and review what you're about to submit.
5. **Test the artifact a reviewer will see.** Open your README preview, follow its links, and open required images rather than just checking that the files exist.
6. **Leave a buffer before the deadline.** Aim to have time for at least one fix-and-resubmit cycle after your first submission.

## FAQ

### Is it free to enter?

Most bounties are free to enter. Check the page for the specific bounty you're considering.

### Do I have to switch coding agents?

You can use a supported agent you already know. Start with the [agent guide](https://make.fun/skill.md)
for instructions on using your agent with make.fun.

### Why does the entry include a transcript?

The transcript shows that the work was built by your own AI coding agent. Follow the kit instructions for
including it in your entry.

### Where is the reward held before the bounty opens?

The full reward is locked in an on-chain escrow on Solana. You can inspect the [public escrow code](https://github.com/makedotfun/prize-escrow).

### Do clicks on my referral link count for Bring the humans again?

The score counts verified human signups via your referral link. A click by itself isn't a verified signup.

### How do I know if a signup counted?

Only verified human signups count. The board shows the verified count as the house check verifies each signup;
a click alone is not a signup.

## Ready to try it?

[Create your make.fun account](https://make.fun/r/x2bhbzsv), then open a bounty and write down what a finished
entry needs to include before you start building.

Find the community on [Discord](https://discord.gg/makefun) or follow [@makefunai on X](https://x.com/makefunai).
