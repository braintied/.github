We build AI so you can be human.

People create in conversation. Agents build and ship. Every company that comes out the other side inherits a back office on day one.

Los Angeles · [braintied.com](https://www.braintied.com) · [kulti.live](https://kulti.live) · [hello@braintied.com](mailto:hello@braintied.com)

<p>
  <img src="loop.jpg" width="880" alt="Talk, build, ship, run." />
</p>

## The north star

Hunger. Housing. Clean water. Renewable energy.

That is the work the money is for. The engine exists so a conversation can become a running company, and so the people who run it can stay human while it does.

## Talk, build, ship, run

A meeting is the start of the company, not a note about one.

| Beat | What happens |
|------|----------------|
| **Talk** | People decide in a room. The system hears the ask and drafts the plan. |
| **Build** | Agents write the product on one shared stack. Humans review. |
| **Ship** | Live URLs, real Stripe, days not quarters. |
| **Run** | CRM, meetings, marketing, finance, and intelligence come with the company. |

The loop ran on air on 16 July 2026: a meeting on Kulti Meet, a landing page built and shipped during the show. [kulti.live](https://kulti.live) is that stage.

## Companies on the engine

| Company | What it is |
|---------|------------|
| [Silver Dollar](https://www.sd4me.com) | Family asset platform. Live. |
| [CoCoach](https://co-coach.app) | AI co-coach for football clubs. Live about six days after the fork. |
| [GuardNIL U](https://www.guardnilu.com) | Development platform for youth athletes and their families. |

Studio work, the portfolio, and the thesis live on [braintied.com](https://www.braintied.com).

## Open source

Two pieces of the engine are public. You run them. They do not log into our machines.

<p>
  <img src="oss.svg" width="880" alt="Watchtower: agent to hook to your server to your Postgres. Research: question and dollar cap to search to cite to a grounded report." />
</p>

### Watchtower

Records what coding agents tried, which of those attempts failed, and the error that came back, so the next session does not repeat the same approach.

It does not call a model. Claude, Grok, GPT, Gemini, Cursor, Codex, OpenCode, or a model on your own machine: if the tool writes a session, Watchtower can store it.

You get hooks, disk adapters, and a small server. Default webhook is `http://localhost:5003/webhooks/session`. The hook refuses `ora-watchtower.fly.dev`. That host is ours.

```bash
git clone https://github.com/braintied/watchtower.git
cd watchtower && npm install && docker compose up --build
```

[Watchtower](https://github.com/braintied/watchtower) · [README](https://github.com/braintied/watchtower/blob/main/README.md) · [AGENTS.md](https://github.com/braintied/watchtower/blob/main/AGENTS.md)

### Research

You name the question and a dollar cap. The engine searches, fetches pages, extracts quotes, synthesizes a report, and grounds every citation against the fetched evidence.

Search and fetch can run at $0 (SearXNG, Crawl4AI). Synthesis needs a model key you supply. Absence of a vendor key disables that lane. It does not silently swap in another.

```bash
pnpm add @braintied/research
```

The host passes credentials in. The package never reads `process.env`.

[Research](https://github.com/braintied/research) · [AGENTS.md](https://github.com/braintied/research/blob/main/AGENTS.md)

Also public, smaller: [agentlog](https://github.com/braintied/agentlog) (session JSON) and [kimi-router](https://github.com/braintied/kimi-router) (Kimi key pool).

The rest of the stack stays private.

## Hire the engine

We will stand up Watchtower or Research for a team: your host, your database, your agents. Studio will take an idea to a live product.

[Consulting](https://www.braintied.com/consulting) · [Studio](https://www.braintied.com/studio) · [hello@braintied.com](mailto:hello@braintied.com)

<p>
  <img src="term.gif" width="880" alt="galien@braintied" />
</p>
