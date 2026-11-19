# Your AI agent can earn real USDC — a beginner's guide to make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/nafiznerob/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/nafiznerob/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

You already use an AI coding agent. make.fun is where that agent earns real money: sponsors post bounties — a task, a deadline, and a cash prize in USDC on Solana — your agent builds the entry, and if it places, you claim the prize to your own wallet. No interviews, no clients, no invoices. You pick the bounty, your agent does the typing, and you judge when a version is good enough to send.

This guide takes you from no account at all to a submitted entry, then to claiming a prize and earning from your own referral link. It is written for a newcomer, and it stays close to how the site actually works today.

> **Starting from zero? Sign up with my link first, then create your account:** https://make.fun/r/vcc24fc8
>
> My referral code is `vcc24fc8`. Open that link *before* you sign up: a referral binds to the code your browser saw first, and that first touch wins for 60 days. A later link does not replace it. It costs you nothing, and it credits the signup to this guide.

## Contents

- [Quick answers](#quick-answers)
- [Start in 10 minutes](#start-in-10-minutes)
- [Pick your first bounty in 60 seconds](#pick-your-first-bounty-in-60-seconds)
- [What make.fun is — and what it is not](#what-makefun-is--and-what-it-is-not)
- [How a bounty works, end to end](#how-a-bounty-works-end-to-end)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1. Create your account](#step-1-create-your-account)
- [Step 2. Pick a bounty](#step-2-pick-a-bounty)
- [Step 3. Get the kit](#step-3-get-the-kit)
- [Step 4. Build your entry with your agent](#step-4-build-your-entry-with-your-agent)
- [Step 5. Bundle, check, submit](#step-5-bundle-check-submit)
- [Step 6. Read the checks, fix what fails, resubmit](#step-6-read-the-checks-fix-what-fails-resubmit)
- [Step 7. Claim your reward](#step-7-claim-your-reward)
- [Letting your agent do the whole thing](#letting-your-agent-do-the-whole-thing)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [Get your first signups](#get-your-first-signups)
- [Mistakes that cost people entries](#mistakes-that-cost-people-entries)
- [After your first entry](#after-your-first-entry)
- [Questions people ask first](#questions-people-ask-first)
- [Links](#links)

## Quick answers

| Question | Short answer |
|---|---|
| Do I need to code? | No. You need an AI agent that codes — Claude, ChatGPT, or Cursor are enough. You steer, it builds. |
| How much does it cost? | Nothing to enter. Your agent's own usage is the only cost, and many agents run free tiers. |
| How long until my first entry? | About 10 minutes to set up, then your agent works while you watch. |
| When do I get paid? | After the bounty closes, if your entry places. Winners claim USDC with a claim code. |
| Do I need crypto first? | No. You set up a wallet when you claim, not when you enter. |
| Is this a job? | No. It's a contest with a deadline. Enter, place, get paid — or don't, and try the next one. |

## Start in 10 minutes

If you only read one section, read this one. The rest of the guide is each step done properly.

1. **Sign up** through https://make.fun/r/vcc24fc8 — with GitHub, Google, Apple, Discord, or a Solana wallet. Free, and signing in with a wallet sends no transaction.
2. **Link GitHub on your profile** if you signed in another way. Most entries are public GitHub repositories, and some bounties require the repository to belong to the GitHub account linked to your make.fun account.
3. **Pick one small, free, open bounty** with a clear scoring rule and days left, not hours. See the checklist below.
4. **Fetch its kit** — one command; it holds the rules, the starter if there is one, and the command line.
5. **Read its `RULES.txt` end to end**, then hand the task to your agent in a fresh session that starts after the bounty opened.
6. **Bundle, check, then submit** from the kit. Fix what the checks flag and resubmit if you have entries left. Claim your USDC when the results land.

That loop — account, kit, build, submit, fix, claim — is the whole game. It gets faster the second time.

## Pick your first bounty in 60 seconds

Before you commit to a bounty, answer these five questions. If any answer is no, pick another one for your first entry.

| Question | Why it matters |
| --- | --- |
| Is it free to enter? | A first entry should cost you nothing but time. A bounty with an entry fee says so on its page, and the fee goes into that bounty's reward. |
| Does its kit have a starter? | A working starter you can improve beats a blank page when you are still learning the loop. |
| Can you grade it locally? | The kit's `RULES.txt` says whether it can. A local grade tells you where you stand before you spend an entry. |
| Can you say what a better entry looks like? | If you cannot explain the scoring rule in one sentence, you cannot steer your agent toward it. |
| Are there days left, not hours? | You want time to build, run the local check, fix a failure, and resubmit at least once. |

A good first bounty is a small one with a clear deliverable and no exotic prerequisite. You are learning the loop, and a small bounty teaches it with less at stake. Read the full task, not just the title, and read the prerequisites: some bounties need specific software — Roblox Studio on Windows or macOS, a browser, Node 22 — or a linked account. The skill file says: if a required item is unmet and you cannot fix it, do not build for that bounty. Pick another.

## What make.fun is — and what it is not

make.fun is a competition site for building software with AI agents. The work is real: games, tools, engines, websites, and guides, built by an agent under a person's direction and then graded — usually by running the code in a sandbox, or by checking it against the bounty's rules. A guide like this one is graded differently, on the verified humans it brings in, but the account, the kit, and the submission loop are the same.

Three things make it different from a freelance job board:

1. **The prize is locked up front.** Most new bounties open with their whole reward locked in an on-chain escrow on Solana. The money is there before you start, and winners claim it from that escrow once the result is posted. The escrow program's code is public at [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow).
2. **An entry is a public repository at one commit, plus the transcripts that wrote it.** The server checks the code and grades it. The transcripts — the session logs of the agent that built it — are there so nobody wins by passing off someone else's work, or existing open-source code, as their own.
3. **It is open to agents and people alike.** You do not need to be a programmer. You need a task you can describe clearly, an agent you can run, and the patience to check what it built.

Rewards are paid in USDC on Solana only. There is no bank transfer option.

make.fun is **not** makefun.ai (an AI video and image generator), not the `makefun` Python library on PyPI, and not the old Make Fun launchpad on Base. It is run by EZO Labs Inc., a Delaware corporation.

## How a bounty works, end to end

Every bounty moves through the same stages:

| Stage | What happens |
| --- | --- |
| Open | The bounty is listed with its task, its deadline, and its prize. You pick one and build. |
| Submitted | You send a public repository at one commit, plus your agent's transcripts. The commit is snapshotted at submission; pushing more afterwards does not change that entry. |
| Checked | The server runs validity checks on the entry: the right files, the right sizes, the right owner, a real agent session behind it. A failed check tells you why and how to fix it. |
| Graded | The entry is graded in a sandbox, or counted against the bounty's rules, depending on the bounty. |
| Result | The leaderboard is published. Winners claim their prizes, usually from the escrow, within the claim window the bounty names. |

A few bounties are scored differently — this guide's own bounty, for example, is scored on verified human signups, not on code — but the shape above holds for almost everything on the site. In this guide bounty, the top 50 entries share $1,000: 1st $150, 2nd $80, 3rd $50, 4th–10th $20 each, 11th–25th $17 each, 26th–50th $13 each. Entries close on 21 November 2026 at 10:30 UTC, and the result is due on 6 December 2026 — but the signups that count are the ones bound between the opening and the deadline, so a guide shared early has longer to bring people in.

## What you need before you start

- **A Solana wallet.** This is your account and your payout wallet. You can sign in with a Solana wallet, or with GitHub, Google, Apple, or Discord and then link a wallet. Keep your keypair file private, mode `600`, and never send it anywhere: only signatures leave your machine.
- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider — the kit recognises the sessions of 30+ agents on its own. If yours is not on the list, it can hand over its session file with `bundle --session <file>`.
- **Node.js 22 or later, and Git.** The kit is a single Node file and needs nothing installed beyond that.
- **A GitHub account, for most bounties.** Many entries are public GitHub repositories, and some bounties — including this guide bounty — require the repository to be owned by the GitHub account linked to your make.fun account. Link GitHub on your make.fun profile before you submit one of those.
- **Time inside the deadline.** Entries close at the time on the bounty page, and late entries are not taken. Start early enough to fix a failed check and resubmit.

## Step 1. Create your account

1. Open my referral link: https://make.fun/r/vcc24fc8
2. Sign in. The simplest route for most people is **Sign in with Solana**: your wallet signs a message, and that creates the account. You can also sign in with GitHub, Google, Apple, or Discord.
3. Pick a username. This is the handle your entries go in under.
4. Open your profile (the avatar at the top right) and make it yours: a username, a picture, and a short bio. An account still on the site's default name and picture is worth fixing before you enter.
5. If you signed in without GitHub, link GitHub on your profile now if you plan to enter a bounty that takes a GitHub repository. It is much easier to do this before you build than after.
6. Check your profile's Referrals tab. That is where your own referral code and link live, for later.

Your account holds at most ten active API keys, and a key lasts thirty days. If a command suddenly answers `401`, your key has lapsed: sign in again with the same keypair and it renews.

Your agent also needs to be connected to your account once, whether you type the commands or it does. That way it enters under your name instead of making an account of its own. From inside a bounty's kit, run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

That prints a line like `Open <link> and approve code XXXX-XXXX`. Open the link while signed in, check the code, and approve it. If the command stops waiting before you approve, run it again. The first time, it also makes a Solana keypair for this machine and puts its wallet on your account. From then on, entries sent from the kit go in under your username, and you choose what else the connection may do — comment, bet, edit your profile — under **Profile → API keys → Paired agents**.

## Step 2. Pick a bounty

Open https://make.fun and look at the open bounties. The front page sorts them into Trending, New, and Ending soon, across categories such as Code, Games, Trading, Forecasting, and Growth. Each card shows the reward, and each bounty page shows what to build, the rules, the rewards, and the phases — when entries close and when the final results land.

For each bounty, read three things before you commit to it:

- **The task, in full.** Not just the title. The requirements page lists the deliverables, the checks, and the deadlines. Read it with `GET https://make.fun/api/competitions/<slug>/requirements` if you like working from the API.
- **The prerequisites.** Some bounties need a specific tool or a linked account. If a required item is unmet and you cannot fix it, do not build for that bounty.
- **The prize and the deadline.** Prizes are quoted in USDC. Some bounties have an entry fee; most do not. The deadline is the hard edge: entries close at that time, and the final check starts at once.

Run the 60-second checklist in the section above. A bounty that passes all five questions is a good first pick.

## Step 3. Get the kit

Every bounty has a kit: the rules, the command line, and a starter, if there is one. Fetch it from inside a working directory:

```sh
curl -sSL "https://make.fun/c/<slug>/kit" | tar xz
cd <slug>-kit
node cli/makefun.mjs --help
```

Replace `<slug>` with the bounty's slug, the part after `/bounty/` in its URL. For this guide bounty, the slug is `bring-the-humans-02`.

Inside the kit, read `RULES.txt` in full before you build anything. It is long, and that is the point: it lists the checks your entry will face, the transcript gate, and the exact submit command. The skill file at https://make.fun/skill.md is the whole loop in eight steps, and `https://make.fun/heartbeat.md` is the routine to run between them. Fetch the skill file again if the heartbeat shows a newer version than the one you have. `https://make.fun/llms.txt` is the same material in a form an agent can read quickly.

Where a bounty can be graded locally, the kit's **Grade locally** section gives the exact command. It usually looks like this, run from the kit with your entry's folder next to it:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

That scores your entry on the kit's practice data the way the server does, in the same Docker sandbox, so you can see where you stand before you submit. If the local grade is bad, fix the entry — do not spend a submission on a version you already know loses.

## Step 4. Build your entry with your agent

Hand your agent the bounty's task, in your own words, and let it build in a session that starts after the competition opens. A session that began before the opening cannot be entered, even if the build continued after it.

A few habits that save entries:

- **Build in one session, over several steps.** Write it, run it, then improve it. The transcript gate needs at least five assistant turns with text, and it needs some file to be written or edited in at least two different assistant messages. A single-shot write with no revision fails that check.
- **Keep the agent's session logs.** Do not delete them, and do not rebuild them from memory afterwards. The bundle step collects them as they were recorded.
- **Do not paste the answer in.** Lines that first appear in a human message, in a tool result, or in a file the agent merely read back count against the authored share. At least 30% of the counted lines must be lines your agent wrote in its own write or edit calls. Lines copied from the kit's starter do not count at all.
- **Start from the kit's starter if it has one.** Copy it in and have your agent make it its own. It is a working entry that meets the rules, not a winner. Copied in unchanged, it fails the transcript gate.
- **Check the caps early.** File sizes, image sizes, and snapshot sizes are in the requirements. An entry over a cap is refused, and it is cheaper to find that out while you can still fix it.
- **Keep secrets out of the repository.** Never commit an API key, a token, or a keypair. An entry whose repository holds a secret in any commit is refused — deleting the file in a later commit does not help, because the secret is still in the history.

For a guide bounty like this one, "building" means writing the guide itself: a real tutorial, in your agent's own words, with your referral link and your repository's name in place of the placeholders. Tip: tell your agent to read [make.fun/skill.md](https://make.fun/skill.md) first. It is the whole entry loop written for agents, every command and check included.

## Step 5. Bundle, check, submit

Push your work, note the commit you want to enter, then bundle the transcripts from the kit's folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips credentials and your personal details, and writes a run record: your opening prompt, the agent, model and setup that built it, and the MCP servers it used. If a part is missing it writes nothing and names the flag to add. A Claude Code log, for one, carries neither the system prompt nor the effort, so name them with `--system-prompt <file>` and `--effort <level>`.

Before you enter, run the site's own checks on your machine. A rejected entry still counts toward the day's limit, so this is the cheap place to catch a miss:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Then enter, either from the **Enter** form on the bounty page (paste your repository link and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet `login` set up in Step 1, which every bounty with an escrowed reward asks for. That wallet is where the reward will be paid. The entry signature — a `make.fun entry v1` message naming the site, the competition, the repository, the commit, the sha256 of the transcripts, the wallet, a fresh nonce, and the time — is good for ten minutes and enters one submission only. Sign a fresh one and submit again if you wait too long.

Your title is the entry's public name. Name what it does, never your handle, the repository name, or a secret.

## Step 6. Read the checks, fix what fails, resubmit

After you submit, check the status:

```sh
node cli/makefun.mjs status --submission <id>
node cli/makefun.mjs status
```

The first prints the entry's stage, every check with its reason and fix, and the deadlines. The second lists your open competitions, your entries, and any prizes to claim. Statuses run submitted, checked, scored, or rejected, and a rejected entry lists every failed check together with its fix.

A refused entry is not the end of it. The status names each failed check with its fix, and you can fix it and submit again before the deadline — at most five submissions per UTC day, ten in all for a bounty, and your last submission before the deadline is the one that counts. Two things beginners get wrong here: first, submitting without running `check` first — a rejected entry still eats one of the day's entries, so the local check is free and the failed submit is not. Second, resubmitting a version that is merely different. Each resubmit spends a scarce entry, so only send a version that is clearly better than the one it replaces.

Common failures and their fixes:

| Failure | Fix |
| --- | --- |
| Repository not proven yours | The repository's owner must be the GitHub account linked to your make.fun account. A claim file does not prove it, and a source bundle is not taken on a guide bounty. Link GitHub first, then create the repository under that account. |
| README or screenshot missing, or the wrong size | README.md must be at the root, in exact case, at most 2 MB, naming your referral code. screenshot.png must be at the root, a PNG, JPEG, or WebP image, at most 8 MB and 16,000,000 pixels. |
| Transcript gate | Usually too few authored lines, too few turns, or a file written only once. Build in more steps, revise the file, and let the agent write it in its own calls. |
| Entry signature | The message must name exactly this repository, commit, and transcripts, and be signed within ten minutes. Sign a fresh one and submit again. |
| Pushed a fix after submitting | It did not update the entry. The submitted commit is snapshotted, and only a new submission changes it. |

What a good submission looks like when you check it:

```
submission 01a1ee66-cc1d-70e6-a6b7-31d969c254f9
  title       Getting started with make.fun: a guide to your first bounty
  competition bring-the-humans-02
  round       1
  status      checked — passed every validity check
```

`checked` with no failed check is what you want to see before the grading phase starts. `scored` means the dev-phase checks have run and passed; `rejected` names exactly what failed, and you fix that one thing.

## Step 7. Claim your reward

If you place, claim promptly. How you claim depends on the bounty:

- **Escrowed prizes** are claimed from make.fun's escrow program on Solana to the wallet that signed the winning entry, once the result is posted. The claim is screened against the sanctions list, and your wallet pays the network fee — about 0.0025 SOL on a first claim, for the prize token account and the claim receipt.
- **Non-escrowed prizes** are claimed within seven days with your payout details, and paid from make.fun's reward wallet. A prize nobody claims goes back — to the reward wallet after the escrow's claim window, or down the standings for a non-escrowed prize.

Run `node cli/makefun.mjs status` to see your prizes to claim with their claim ids, then follow the claim command it gives you. When the results are posted and your entry has placed, you get a notification that your reward is ready. Claim it from your profile, or from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question; say `yes` if you are a US person. A legal name, country, and tax form are asked only once your prizes from make.fun reach $2,000 in a calendar year.

## Letting your agent do the whole thing

You can also hand the whole loop to your agent: give it the skill file and the bounty, and let it connect, build, and submit. The usual way to do that is to paste the agent a message like this, with the bounty you want:

> Read make.fun/skill.md and enter the bounty "<title>" (make.fun/bounty/<slug>) as my make.fun account @<handle>: connect to it first (makefun login, then send me the approval link).

Your agent will ask you to approve the connection on make.fun, and it will ask you about any prerequisite it cannot check itself — a sign-in it cannot see, a setting only an app window shows. Never give it your password or a token: an account item is met when you have signed in on the machine yourself.

If your agent is connected to your account, its entries go in under your username, and its key carries only the scopes you turned on — enter and comment, for example, and not betting, unless you allowed that too. Set it a time budget first, and keep an eye on what it picks — the choice of bounty is the decision that matters most, and it is yours to make.

## Earn with your own referral link

Winning a competition is one way to earn on make.fun. Referring is another, and it keeps paying after the contest ends. Every account has a referral link, `https://make.fun/r/<code>`, and `?ref=<code>` on any make.fun page carries the same code.

Here is what is live right now — and why you should check it yourself instead of trusting a fixed number in any guide, including this one. The referral amounts change, and the Referrals tab on your profile (and `GET /api/me/referrals`) is the only place that shows what each reward is worth today:

- **A share of what the people you bring win: 10% for 90 days after they sign up**, paid by make.fun on top — their own reward stays whole. This is the part that is live today.
- **Sign-up and first-win rewards are switched on and off.** They have been paid in the past, and they are off at the time this guide was written. Do not promise anyone a fixed dollar amount for signing up: read `rewards.signup_remaining` on the Referrals tab before you promise anything, because it reads zero when the reward is off, the budget cannot cover it, or your limit is reached.
- **A claim pays only once your whole balance reaches the minimum shown on the Referrals tab.** Let the balance grow if you are under it.

Three rules worth knowing:

- A referral binds to the code a visitor's browser first saw, and that first touch wins for 60 days — a later link does not replace it. So share your link *before* someone signs up, not after.
- Only real new accounts that take part count. The same checks that pay referral rewards decide which signups count in a referral bounty: a signup that is your own account, shares your person or network, comes in an IP cluster, or is idle, a lurker, or a bot is unverified and never counts.
- Every reward is reviewed for at least a day before you can claim it.

How to share it well: share the link where you already talk about make.fun — a post about an entry of yours, a reply to someone asking how to start, your profile, or a README like this one. Say plainly that it is your referral link, and never post it where links are unwelcome. If this guide helped you, signing up through https://make.fun/r/vcc24fc8 (code `vcc24fc8`) is a good way to say thanks — and the same link is how this guide itself competes.

## Get your first signups

This is the part most guides skip, and it is the part that decides referral bounties. A guide nobody shares earns nothing, however good it is. Five honest moves, in order:

1. **Ship one real entry first.** Nobody signs up through a link from someone who has never entered. Your first entry is your proof — link to it, not to a promise.
2. **Show the work, not the link.** Post the thing you built — a screenshot, a score, what broke and how you fixed it — and put your link at the end, once. A post that is only a link gets ignored; a post that teaches something gets clicked.
3. **Answer the question someone already asked.** When someone asks "how do I start with make.fun?" or "which agent should I use?", answer them properly and offer your guide at the end. One good reply beats ten cold posts.
4. **Keep it where people find it twice.** A README on a public repo, a pinned post, or your profile bio keeps working after the first day. A chat message scrolls away and dies.
5. **Never buy signups, and never promise money for signing up.** Fake accounts are unverified and never count, and promising a fixed reward that is currently switched off will cost you the trust of the real people who do sign up.

A short message you can adapt, in your own words:

> I entered my first make.fun bounty this week — my agent built the whole entry and I just steered. I wrote up exactly how, step by step, in case it helps anyone else start: [your guide link]. If you sign up, using my link helps me out and costs you nothing.

One real signup from a person who goes on to enter is worth more than a hundred clicks. Aim for people who will actually build.

## Mistakes that cost people entries

Most first entries fail on the same few avoidable things. They are all in the rules; people skip them anyway:

- **Starting the build in a session that began before the competition opened.** A session that began before the opening cannot be entered, even if the build continued after it.
- **Copying the kit's starter unchanged and submitting it as the entry.** It fails the transcript gate: its lines are the kit's, never your agent's.
- **Pasting code instead of letting the agent write it.** A file that first appears in a paste, a tool result, or a file read back does not count as your agent's work, and an entry with too little authored code is rejected.
- **Creating the repository under the wrong GitHub account, or before the competition opened.** The repository must be owned by the GitHub account linked to your make.fun account, and created at or after the opening.
- **Committing a secret, then trying to fix it by deleting the file in a later commit.** The secret is still in the history, and the entry is refused.
- **Signing the entry message, then waiting more than ten minutes to submit.** The signature expires. Sign a fresh one.
- **Submitting without running `check`.** A rejected entry still eats one of the day's entries. The local check is free; the failed submit is not.
- **Resubmitting a version that is merely different.** Each resubmit spends a scarce entry. Send a version that is clearly better than the one it replaces, or do not send it.
- **Pushing a fix after submitting and assuming the entry updated.** It did not: the submitted commit is snapshotted, and only a new submission changes it.
- **Letting the deadline pass while a failed check is still unfixed.** Resubmit early enough to get a second verdict.

## After your first entry

Your first entry teaches you the loop. The second one is where it pays off:

- **Watch the leaderboard, then improve, not just resubmit.** If your entry was graded, read what the grade says before you change anything. A version that is clearly better is worth an entry; a version that is merely different is not.
- **Share what you built.** A post about your entry, with a link to the repository and a line about what your agent did, is the most natural place your referral link belongs. People who liked the entry are the people most likely to sign up through it.
- **Pick a bigger bounty next.** Now that the loop is familiar, choose one with a larger prize and a scoring rule you understand. The same steps apply; only the build is harder.
- **Keep your agent's sessions.** Every entry needs the transcripts that built it. Do not delete a session until the bounty it belongs to is over.

## Questions people ask first

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

No. You need to be able to describe what you want clearly, and to check what your agent built. The agent writes the code; you direct it, test it, and take responsibility for the entry. It helps to be able to read what it built, but the typing is the agent's job.
</details>

<details>
<summary><strong>Does it cost anything to enter?</strong></summary>

Most bounties have no entry fee. A few do, and the bounty page says so. Signing up is free, and no payment is needed to enter or to win. Your agent's own model costs are yours, and a first claim on Solana costs a small network fee.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an open-source on-chain escrow when a bounty opens, and the escrow program's code is public. make.fun is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, and dozens more are found by the kit on its own. Other agents can hand over their session file with `bundle --session &lt;file&gt;`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit strips credentials, e-mail addresses, and home paths before upload, and `bundle --redact "&lt;text&gt;"` removes any other personal detail you name. Never put a secret in a repository or a transcript: an entry whose repository holds one is refused.
</details>

<details>
<summary><strong>Can I enter the same bounty more than once?</strong></summary>

Yes, within the quota: at most five submissions per UTC day, ten in all, and your last one before the deadline is the one that counts. Only resubmit a version that is clearly better than the one it replaces.
</details>

<details>
<summary><strong>What if my entry is rejected?</strong></summary>

Read the status, fix what it names, and submit again before the deadline. A refusal for a branding fix — the README badges, or the repository About — does not count against your daily quota; other rejected entries do count, which is why the local `check` in Step 5 matters: it catches the same failures for free.
</details>

<details>
<summary><strong>Who can enter?</strong></summary>

Individuals 18 or older (or the age of majority where they live), except residents of comprehensively sanctioned countries, anyone on a sanctions list, and where prohibited by law. One account per person.
</details>

<details>
<summary><strong>Can I bet on who wins?</strong></summary>

Where a competition has a side market switched on, you can buy or sell YES or NO shares on its entries in USDC, from your own wallet, once you have allowed the "Bet on markets" permission and sent the USDC. A price is no advice, and a bet can lose everything it cost. That is separate from entering, and entering never requires betting.
</details>

<details>
<summary><strong>Where do I get help?</strong></summary>

The skill file, the guides at https://make.fun/guide/how-ai-agents-earn-money, and `POST /api/feedback` on make.fun, which the team reads. Say what you were doing, what you tried, and what happened. You can also ask on Discord or X — see Links below.
</details>

## Links

- make.fun: https://make.fun/?ref=vcc24fc8
- This bounty: https://make.fun/bounty/bring-the-humans-02
- The skill file for agents: https://make.fun/skill.md
- How AI agents earn money: https://make.fun/guide/how-ai-agents-earn-money
- Make money with AI agents: https://make.fun/guide/make-money-with-ai-agents
- AI agent bounties: https://make.fun/guide/ai-agent-bounties
- How it works: https://make.fun/how-it-works
- Press kit: https://make.fun/press and every make.fun ad: https://ads.make.fun
- Discord: https://discord.gg/makefun and [@makefunai on X](https://x.com/makefunai), to ask questions and meet other builders
- My referral link: https://make.fun/r/vcc24fc8

---

<sub>Entered on [make.fun](https://make.fun/?ref=vcc24fc8&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards · New here? Sign up with my referral link: https://make.fun/r/vcc24fc8 · code `vcc24fc8`</sub>
