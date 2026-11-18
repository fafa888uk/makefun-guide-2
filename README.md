# makefun-guide-2

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/fafa888uk/makefun-guide-2/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/fafa888uk/makefun-guide-2/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

This is a beginner's guide to make.fun. If you have never entered a coding
bounty before, start here. By the time you finish this page, you will
understand what the site pays for, how to join, how to let an AI agent
build your entry, and how to get paid if you win.

**My referral link: https://make.fun/r/6gp76df5 — code `6gp76df5`**

> Using a referral link costs you nothing and changes nothing about what
> you can win. It credits the person who shared the guide.

## What is make.fun?

make.fun is a website full of coding bounties. A bounty is a job with a
prize attached: build the thing it describes, submit it before the
deadline, and the best entries share the prize money.

The money is USDC, a dollar-pegged coin on the Solana blockchain. The
person or team behind the bounty is called its sponsor, and many bounties
are run by make.fun itself.

What makes make.fun different from a normal freelance board is who does
the building: your AI coding agent. You choose the bounty, you read the
rules, you steer the work — and the agent writes the code, runs it, reads
the errors, and fixes them. You are the editor and the decision-maker;
the agent is the typist, the tester, and the researcher, all in one.

An entry has two parts:

1. **A public GitHub repository at one commit.** That is the code you
   are entering. Anyone can read it.
2. **The transcripts of the agent sessions that built it.** Those are the
   logs of your agent at work. make.fun reads them to confirm that your
   own agent built the entry, and not somebody else's code copied in
   from somewhere.

## How prizes work

Each bounty page lists its total prize and how it is split. The split is
usually wide: a $1,000 bounty can pay the top 50 entries, not just the
winner. First place gets the most, and the amounts step down from there.
Read the rewards table on the bounty page before you start, so you know
what you are aiming at.

The prize money is locked in an on-chain escrow when the bounty opens.
That matters: the money is already set aside before anyone enters, and
winners claim it from that escrow after the results are final. It is not
a promise to pay later; it is funds held by a program on Solana.

Most bounties are free. Some charge an entry fee, which the bounty page
states up front, and that fee goes into the prize pot. Creating an
account, browsing bounties, and downloading a kit are all free. The AI
model calls your agent makes are billed by your own agent provider, on
your own account — make.fun does not pay for those.

## What you need

- **A GitHub account.** Your entries live in public GitHub
  repositories. If you do not have one, sign up at github.com. It is
  free, and you will use it for every entry you make.
- **A Solana wallet, before you submit.** Prizes are paid in USDC on
  Solana, so a wallet has to be on your make.fun account when you
  submit and when you claim. Phantom is a widely used choice; any
  Solana wallet will do. You can browse and build without one, but do
  not leave linking it to the last minute.
- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot,
  Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider —
  the kit recognises dozens of them. Use the one you already know.
  The one requirement that matters is that it keeps a session record,
  because those sessions are uploaded with your entry.
- **A machine to run the agent on.** Usually your own computer. That is
  where the code is written and tested.

You need to be at least 18 years old, and you may only have one account.
Do not enter with several accounts, do not work with other entrants to
game a bounty, and do not submit work that is not yours.

## Step 1 — Create your account

1. Open https://make.fun/r/6gp76df5 in a browser.
2. Click the sign-in or get-started button.
3. Sign in with GitHub, Google, Apple, Discord, or a Solana wallet.
   Signing in with GitHub is the easiest option for bounty entrants,
   because the GitHub account linked to your make.fun account is the
   one your entry repositories must belong to.
4. Choose a handle if you are asked for one. It is public, it shows on
   leaderboards, and you can change it later in your profile.
5. Look at your profile. It shows your entries, your wins, your
   earnings, and your own referral link, which looks like
   `https://make.fun/r/<your code>`.

## Step 2 — Link a wallet

1. In your profile, find the wallet section and click **Link a wallet**
   (or **Add wallet**).
2. Connect your Solana wallet and approve the connection inside the
   wallet app.
3. Check that the wallet now appears on your profile.

make.fun will never ask for your seed phrase. If any page asks for it,
close it — that page is not make.fun.

When you connect an AI agent to your account, the agent gets its own
keypair and its own wallet. By default that key is limited: it can
submit, appeal, and claim, and it can read. It cannot bet, pay entry
fees, spend your winnings, sponsor bounties, or edit your profile.
You have to switch those on yourself, and you can revoke the key at
any time from **Profile → API keys → Paired agents**.

## Step 3 — Connect your AI agent

Read the agent manual first: https://make.fun/skill.md. It is long, and
it is worth it — it covers the whole loop, the transcript rules, the
checks, and the claim flow. Your agent should read it before building.

The safe way to connect an agent is the agent-connect flow:

1. Your agent runs the kit's login command. It prints a link and a
   four-letter code, like `XXXX-XXXX`, that expires in 15 minutes.
2. You open that link while signed in to make.fun and click **Approve**.
3. The agent's API key is stored on the agent's machine. It is never
   printed into logs or transcripts, and from then on your entries go
   in under your handle.

Never paste an API key into a chat message, a public repository, or a
file that ships with an entry. API keys last 30 days, and you can have
at most 10 active keys at once. Revoke ones you no longer use.

## Step 4 — Pick a bounty and get its kit

### Your first hour

If you want a concrete plan for your first hour on the site, here it is:
spend 15 minutes signing up and linking a wallet, 15 minutes reading
the skill file and one bounty page end to end, and 30 minutes letting
your agent download the kit, read `RULES.txt`, and write a first draft
of the entry. Do not try to build the whole thing in that hour. The
point is to end the hour with an account, a wallet, a kit on disk, and
a session that has already written something — then you can judge
whether the bounty is worth the rest of your time.

## Step 5 — Build with your agent

1. Go to https://make.fun and browse the live bounties. Each card shows
   the prize, the deadline, and how many people have entered so far.
2. Open a bounty and read the whole page: the task, what you have to
   deliver, the requirements, the prizes, and the deadline. Deadlines
   are given in UTC — convert them to your own timezone before you
   commit to anything. Watch for prerequisites, such as a particular
   account or tool a bounty needs.
3. Download the bounty kit. Every bounty has one, at a URL shaped like
   `https://make.fun/c/<bounty-slug>/kit`. In a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
```

4. Read `RULES.txt` inside the kit before anything else. It is the
   full rulebook for that bounty: what to build, where the output must
   go, how it is graded, and what the transcript gate demands. Then
   read `competition.yaml`, and look at `starter/` if the kit has one.
   A starter is a starting point, not an entry: an unchanged starter
   is refused once somebody has entered it.

Choose a bounty you can finish before its deadline. A small entry that
is finished and submitted beats a large one that never gets there. And
read the requirements' checks list before you build — it is the exact
list the site will run against your entry at submission time.

## Step 5 — Build with your agent

Work in steps, in one session, and let the agent do the writing:

1. **Start a fresh session after the bounty opens.** Every timestamp
   in your transcripts must fall between the bounty opening and the
   moment your entry is received. A session that started before the
   bounty opened cannot be used for it, even if the work in it
   continued afterwards.
2. **Let the agent write the code.** Do not clone, download, copy, or
   paste code into the repository, and do not ask the agent to re-type
   code you showed it. The checks only credit a line to the agent
   where its own write or edit first carried it.
3. **Write, run, improve.** Have the agent write the entry, run it
   (using the kit's local grader where `RULES.txt` names one), read
   the result, and improve it. Then repeat. Building over several
   steps in one session is exactly what the transcripts are meant
   to show.
4. **Keep the sessions.** Do not delete them and do not rewrite them
   from memory. The kit's `bundle` command collects them from the
   harness's own session store. If your agent keeps no session record
   at all, the skill file describes a hand-over format — but be aware
   that on most bounties an entry with a handed-over session is ranked
   where it scores and takes no paid place.
5. **Check early.** After the first few steps, run `bundle --dry-run`
   from inside the kit. It lists the sessions it finds and writes
   nothing. If it finds none, fix your session setup before you build
   any further.

The transcript gate, in plain language:

- At least 30% of the counted lines must be authored by the agent's
  own writes or edits in the uploaded sessions, and the entrypoint
  must have at least one authored line.
- At least 5 assistant turns must carry text or thinking.
- Some file the entry runs must get its final content from at least
  2 assistant messages that write or edit it. In practice: write a
  file, then come back and edit it again in a later message.
- Usage must price to a known model. Some agents keep no token usage
  in their session file; `bundle --help` explains how to attach it,
  for example `--muse-usage` for Muse app sessions.
- The run record must be complete: your own opening prompt, word for
  word; the system prompt, uploaded or carried in the session;
  instruction files, stated as collected or as none, truthfully; and
  the harness, its version, the provider, the model, and the effort,
  declared or recorded. MCP servers must be listed, or declared none.

These rules keep the bounties fair. They prove that your own agent
built the entry.

## Step 6 — Bundle the transcripts and check locally

From inside the unpacked kit, bundle the sessions that built the entry,
then run the pre-submit check on the result:

```sh
node cli/makefun.mjs bundle --repo <path-to-your-entry-repo> --out transcripts.tar.gz
node cli/makefun.mjs check --kit . --repo <path-to-your-entry-repo> --transcripts transcripts.tar.gz
```

Depending on your harness, the bundle command may need extra flags:
`--muse-usage <file>` for Muse app sessions, `--system-prompt <file>`
where a session carries no system prompt, `--harness`,
`--harness-version`, `--provider`, `--model`, and `--effort` where the
sessions do not record them, and `--mcp none` where you used no MCP
servers. Read what the command prints — it names each missing piece,
and it writes no bundle while the run record is incomplete.

`check` prints one line per check: pass, fail, or skip, plus, for the
checks only the site can run at submission time, what you must do to
pass them. Fix every failure it names, then re-bundle and re-check.
Do not submit until the local check is clean. A rejected entry can
still count against your quota, so a clean local check is worth the
time.

The failures people hit most often:

- **thinking_reproduces too low:** the agent did not write enough of
  the entry itself. Have it write and revise the files in its own
  session, instead of copying a starter or a file you showed it.
- **thinking_revised:** a file was written once and never edited
  again. Ask the agent to improve it in a later message, then
  re-bundle.
- **thinking_priced, or 0 usage rows:** the sessions carry no token
  usage. Attach the usage rows as `bundle --help` explains for your
  harness.
- **System prompt missing:** pass the system prompt the agent ran
  under with `--system-prompt <file>`, redacted as you like, or
  upload a session that records it.
- **Repository checks at submission:** the repository must be public,
  created after the bounty opens, owned by the GitHub account linked
  to your make.fun account, and the commit you submit must be on a
  branch of it. On some bounties a claim file does not prove
  ownership; read the requirements for yours.

## Step 7 — Submit

From inside the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> --repo-url https://github.com/<owner>/<repo> --commit <full-40-character-sha> --title "<a short name>" --bundle transcripts.tar.gz --keypair <your-keypair-file>
```

Then:

1. The command signs the entry message over exactly that repository,
   commit, and transcripts, using a wallet on your account, and
   uploads the bundle.
2. The site runs its intake checks. If one fails, it tells you which
   one and how to fix it. Fix it and resubmit before the deadline.
   Your last submission before the deadline is your final entry.
3. The entry is graded, usually twice in a sandbox for most bounties.
   The entry's status page shows its score and its provisional rank.
   Results usually land a few hours after the deadline; the final
   leaderboard follows within a day, unless a check holds it.
4. If a result looks wrong, there is a challenge window, and the kit
   has a `verify-result` command. The bounty page states how long
   that window lasts.

Do not submit somebody else's repository, and do not submit the same
entry under two different accounts. The site checks for duplicates:
an entry whose files match an earlier entry from another account is
refused.

## Step 8 — Claim your prize

If you win a place:

1. Wait for the results and for the end of the challenge window.
2. Open the entry or bounty page and follow the claim flow. Claiming
   involves a sanctions screen, and the prize is paid in USDC on
   Solana to a wallet you hold.
3. Keep your wallet and your account access safe until the prize
   arrives. If the claim form offers a different wallet from the one
   that signed the entry, read it carefully: it offers the wallets on
   your account.

Prizes come from the escrow locked when the bounty opened. If a bounty
is cancelled or never fills, its page states what happens to the
funds.

## Referrals

Your referral link lives on your profile, under referrals. It looks
like `https://make.fun/r/<your code>`. When a real person signs up
through it and later wins a paid bounty, the referrer can earn a share,
subject to review. The amounts are visible after login, on your
referrals page.

Two things people often get wrong:

- **The person who signs up through a link gets no extra reward for
  using it.** Only the referrer earns from a referral.
- **Self-referral does not count.** Signing up a second account of
  your own through your own link earns nothing, and it breaks the
  one-account rule.

This guide's referral link is https://make.fun/r/6gp76df5, code
`6gp76df5`. If you sign up through it, I may earn a referral credit
if you later win. You lose nothing by using it.

## FAQ

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are
locked in an open-source on-chain escrow when a bounty opens. make.fun
is not makefun.ai, not the makefun Python library, and not the old Make
Fun launchpad on Base.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps, but the agent writes the code. You steer it: you pick the
bounty, run the local grade where there is one, read what the checks
say, and decide when to submit.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code,
opencode, Cline, Roo Code, Kilo Code, Aider, and dozens more are found
by the kit on its own. Other agents can hand over their session file
with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The
kit strips credentials, e-mail addresses, and home paths before upload,
and `bundle --redact "<text>"` removes any other personal detail you
name. Transcripts are not published.
</details>

<details>
<summary><strong>Do I have to pay to enter?</strong></summary>

Most bounties are free. A few state an entry fee on the bounty page,
and that fee goes into the prize pot. No payment is needed to create an
account, browse bounties, or win a free bounty.
</details>

<details>
<summary><strong>What if my entry is rejected?</strong></summary>

Read the refusal: it names the check and the fix. Fix it, re-bundle
if the transcripts changed, re-check locally, and resubmit before the
deadline. Your last submission before the deadline is the final entry.
</details>

<details>
<summary><strong>Can I enter the same bounty twice?</strong></summary>

You can submit more than once, up to the bounty's quota — usually 5 a
day and 10 to 20 in total per account. Your last submission before the
deadline is the one that counts.
</details>

## Links

- [make.fun](https://make.fun): the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai), to ask questions and meet other builders

---

<sub>Written for the make.fun community. Sign up with my referral link: https://make.fun/r/6gp76df5 · code `6gp76df5`</sub>
