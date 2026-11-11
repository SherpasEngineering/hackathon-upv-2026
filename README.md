<p align="center">
  <img src="assets/banner.png" alt="Bring the plan to life. Sherpas x UPV Sigma Data Club, 12 to 19 November 2026" width="100%">
</p>

# Bring the plan to life

**Sherpas x UPV Sigma Data Club hackathon, 12 to 19 November 2026**

## Join the Discord first

<a href="https://discord.gg/wVUZXmxdS"><img src="assets/discord-qr.png" alt="QR code: join the Discord" width="160" align="right"></a>

**[Sigma Data Club x Sherpas Wealth on Discord](https://discord.gg/wVUZXmxdS)** is where everything happens during the week. Scan the code or click the link:

- **Announcements and rules** for the hackathon
- **Access details** for the MCP and your team's AI key
- **Questions to Sherpas mentors**, answered 13 to 18 Nov in the Sherpas challenge channel
- **Hand-ins**: your Friday idea and your final work

Every team member should join before the kick-off on 12 Nov.

## Start here

1. Read the brief below: the challenge, cases, tools and hand-ins are all on this page.
2. Click **Use this template > Create a new repository** (top right on GitHub). One person per team does this, under their own account.
3. In your new repo, go to **Settings > Collaborators** and add your teammates.
4. Look at the cases in [`cases/`](cases/) and build.

Your repo is yours: any language, any framework, any structure. Delete or rewrite anything here, but keep a README that says what you built and how to run it.

## Who we are

Sherpas Wealth is the first AI Growth Platform for financial advisors ([sherpaswealth.com](https://sherpaswealth.com)). Advisors are our customers. Families are their clients.

For every new client, an advisor does three jobs:

| | Job | Today |
|---|---|---|
| 1 | **Collect the data**: who the family is, what they earn, own and owe, and what they want | Solved by Sherpas: our **Intake** agent reads any document and fills in the client |
| 2 | **Do the math**: turn that data into a plan, with clear recommendations | Solved by Sherpas: **Paraplanner** and **Portfolio analyst** do the analysis. 8 hours of work becomes 20 minutes per client |
| 3 | **Explain the plan**: walk the family through it and answer their doubts | **Still done by hand, one meeting at a time.** This is your challenge |

## The challenge

**Bring the plan to life.** Take a family from their plan to understanding it and wanting to act on it: like having an advisor in the room, or better.

Design for either situation: families who will meet an advisor later (they arrive already understanding their plan), or families who never will (the plan has to land on its own).

What success looks like:

- **It captivates.** It grabs their attention in seconds, and holds it.
- **They get it.** It works for someone who knows nothing about finance, and for someone who knows a lot.
- **Made for them.** It feels personal and relevant to this family, and to each person in it.
- **They act.** They want to take the first step, and keep coming back until they do.

Any format, any channel, any device. Sherpas already has guided tours and a chat on the plan: if your idea is only one of those, it scores low on creativity. Use them as a starting point and go further.

**Bonus, the days after:** people think it over, forget, and come back with new questions on day 3 or day 30. If your idea covers those days too, even better.

### How families receive advice today

The family shares their goals and financial information. Sherpas produces an online plan with an overview, recommendations and projections. Days or weeks later, the advisor usually explains it in a screen-sharing meeting. Advisors would rather spend that time on the family's questions, fears and decisions.

Even a clear plan is a lot to take in alone. Partners may want different levels of detail or different ways of learning. After the meeting, families often need time and follow-up before acting. Your experience can help before, during or after that conversation.

## The cases

Four synthetic households, true to life, built for this hackathon. Each one has a complete Sherpas plan, from a financial health score of 26 to 82 out of 100.

| Family | Score | Who they are | Their story | Files |
|---|---|---|---|---|
| Timothy & Melanie Weah | 60 | 40 and 38, Liam (6) and Josh (3). An $18,000 credit card at 18% and a $15,000 student loan. $150,000 in cash, 401(k)s, Roth IRAs, a brokerage account, a $350,000 home. San Francisco, CA | Plenty of cash and an expensive card at the same time. Where should each dollar go? | [`cases/timothy-melanie-weah/`](cases/timothy-melanie-weah/) |
| Michael Carter | 26 | 37, $180,000 salary, renting. Austin, TX | Wants a $550,000 home in 2027 and to retire at 58. Can he do both? | [`cases/michael-carter/`](cases/michael-carter/) |
| Daniel & Emily Johnson | 52 | 44 and 42, two kids, a $560,000 mortgage, an $18,000 card at 24.9%. Denver, CO | College for Oliver and Sophia, and retirement at 62. What comes first? | [`cases/daniel-emily-johnson/`](cases/daniel-emily-johnson/) |
| Samantha Lewis | 82 | 47, two teenagers, $250,000 salary. Miami, FL | Debt-free and well insured. College bills start now and a second home in 2030. What next? | [`cases/samantha-lewis/`](cases/samantha-lewis/) |

Each family folder contains only the plan data and, where available, its current PDF report:

| File | What it contains |
|---|---|
| `financial-health.json` | Who the family is, their score and why, their financial profile, figures and key metrics, written analysis and yearly projection |
| `investment-analysis.json` | Accounts and holdings, figures and key metrics, and the written investment analysis |
| `report.pdf` | The client report, where a current version is available |

All amounts are US dollars. The JSON files contain the current plans for all four families. PDFs are included for Timothy and Melanie, Michael, and Daniel and Emily. Samantha's PDF is not included yet.

Use the data from any language or framework. No application code is included.

## Your tools

| | |
|---|---|
| **4 cases through the MCP** | Read-only access to the four families and their plans, with a secure login. Access details on Discord |
| **Discord mentors** | Sherpas mentors answer your questions, 13 to 18 Nov |
| **50 € per team in AI credits** | For the models you choose, through our AI proxy (below) |
| **Anything else** | Any stack, any model, any device |

### Access

Connection instructions and your team's AI key are shared on Discord. The services are:

- Cases MCP: `https://mcp-hackathon.sherpaswealth.com/mcp`
- AI proxy: `https://llm-hackathon.sherpaswealth.com`

For code access to the MCP, get a personal token at [the login page](https://mcp-hackathon.sherpaswealth.com/personal-token) using your UPV email. Tokens last 72 hours. The MCP provides `list_cases` and `get_case`.

Keep access keys and tokens private and on your backend. Never commit them or include them in browser code.

### Models and usage prices

These are the model names to use with the hackathon proxy. Prices below are the proxy's configured usage rates, checked 11 November 2026, in US dollars. They are charged against your team's credits. Input is what you send; output is what the model generates.

| Model | Mode | Input / output per 1 million tokens |
|---|---|---|
| `deepseek-flash` | Text | $0.30 / $1.20 |
| `gemini-3.5-flash-lite` | Text | $0.30 / $2.50 |
| `gpt-5-mini` | Text | $0.25 / $2.00 |
| `gpt-realtime-2.1-mini` | Voice | $10 / $20 for audio; $0.60 / $2.40 for text |
| `gpt-realtime-2.1` | Voice | $32 / $64 for audio; $4 / $24 for text |
| `gemini-3.8-live` | Voice | $3 / $12 for audio; $0.75 / $4.50 for text |
| `gpt-live-1` | Voice | $0.05 per minute of session time |

Token counts differ across models, so these rates do not directly compare the cost of an identical conversation. Cached input may have a different rate. Start with a small test and check your team's usage.

- **Text:** OpenAI-compatible `POST /v1/chat/completions` at the proxy address.
- **Realtime voice:** WebSocket `/v1/realtime?model=MODEL_NAME`, for the Realtime models and Gemini Live.
- **GPT Live:** WebSocket `/v1/live/sessions`, with a different protocol from Realtime.
- **Team limits:** 60 requests per minute and 4 concurrent requests or sessions.
- **Budget:** the proxy records spend in USD. Your issued team key sets the spending allowance. Check usage through the authenticated `/key/info` endpoint, which returns `info.spend` and `info.max_budget`.
- **Voice sessions:** close them when finished. Voice usage is recorded when a session closes, so a long session can exceed the remaining allowance before the limit takes effect.

## Your week, and what you hand in

| When | What |
|---|---|
| 12 Nov, 15:00 | **Kick-off.** The challenge and an MCP class, building 1E, room 2.3 |
| 13 Nov, 22:00 | **Your idea.** A private message to the mentors on Discord, one page max, in bullets: what you will build (2 to 3 lines) and why; what you considered and ruled out, and why. Send it as soon as you know. You can still change your mind later. Counts a little in the score |
| 18 Nov, 23:59 | **Hand in, on Discord:** your GitHub repo; a working MVP; a 2-minute video, recorded however you like (screen recording, or your phone pointed at the screen; it does not count in the score, it lets us see your work before demo day); a paragraph on what you built and why (half a page to one page) |
| 19 Nov, 12:45 | **Demo day.** A two-minute pitch per team, then prizes, same room |

## How we judge

Six questions, 100 points:

| Points | Criterion | The question we ask |
|---|---|---|
| 20 | Captivating | Does it grab their attention, and hold it? |
| 20 | Understanding | Would it work for someone new to finance, and for an expert? |
| 20 | Motivation to act | Would they want to act, and keep coming back until they do? |
| 15 | Personal | Does it feel made for them, and for each of them? |
| 15 | Creativity | What did it add that we did not ask for? |
| 10 | Your Friday plan | A clear choice, and honest about what you ruled out and why? |

Getting every figure exactly right does not count in the score: Sherpas already does that inside the product. Use the case data, avoid inventing numbers, and spend your time on the experience.

## Prizes

<p align="center">
  <img src="assets/join.png" alt="Sherpas wants you. Internship opportunities" width="100%">
</p>

Sherpas is looking for talent. The best prize is building real things with us: internships for the teams that stand out.

And there is cash: **1st 600 €**, **2nd 250 €**, **3rd 150 €**.

## A few financial terms

- **Net worth:** what the family owns minus what it owes.
- **Cash flow:** money coming in minus money going out.
- **Liquidity:** money available to use quickly.
- **401(k) and IRA:** US retirement savings accounts.
- **Roth:** an account funded with after-tax money, with tax-free qualifying withdrawals.
- **529:** a US education savings account with tax advantages.
- **Living map:** a year-by-year view of the family's projected financial life.
