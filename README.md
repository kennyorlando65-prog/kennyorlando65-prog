# Joshua Ubah

Full-stack software engineer. I build production web applications with Next.js, React, TypeScript, Supabase and Node.js, and I am building toward AI/ML engineering.

I care about the parts of a system that are easy to skip: the data layer, the authorization model, and what happens when a request arrives twice.

## What I build

Web applications that hold real data and real money, end to end. Frontend, API, database, auth, deployment.

The work I am most interested in is the unglamorous half: Row Level Security policies that actually hold, prices that are computed on the server instead of trusted from the browser, fulfilment that is safe to retry, and CI that fails before a bug reaches production.

## Stack

**Languages** — TypeScript, JavaScript, Python, SQL, HTML/CSS

**Frontend** — React, Next.js (App Router), Tailwind CSS

**Backend** — Node.js, Next.js server routes and server actions, FastAPI, Supabase Edge Functions (Deno)

**Data** — PostgreSQL, Supabase, Row Level Security, versioned SQL migrations

**Platform** — Vercel (including Services), GitHub Actions, Supabase

## Selected work

| Project | What it is | Stack |
| --- | --- | --- |
| [intelligencegrid](https://github.com/kennyorlando65-prog/intelligencegrid) | Open-source global intelligence and situational-awareness platform. Fourteen analysis modules over free, key-less public sources, built around one commitment: it reports how well it can see a territory, not just what it found there. A quiet region is labelled *thinly observed*, never *calm*. | Python, FastAPI, Next.js, TypeScript |
| [crypto-anomaly-detector](https://github.com/kennyorlando65-prog/crypto-anomaly-detector) | Statistical anomaly detection over CoinGecko's free public data. Rolling z-scores, volume spikes and volatility regime change, with a backtest that reports how many alerts would have fired. Statistics, not machine learning — no trained model and no price prediction. | Python, FastAPI, Next.js, TypeScript |
| [nuvora-2.0](https://github.com/kennyorlando65-prog/nuvora-2.0) | White-label digital services platform. Server-side pricing, RLS from migration one, idempotent fulfilment, supplier adapters behind one interface. | Next.js, TypeScript, Supabase |
| [leviathan-app](https://github.com/kennyorlando65-prog/leviathan-app) | On-chain whale intelligence. Multi-chain event ingestion, tiered access, Telegram delivery, scheduled polling. | TypeScript, Supabase Edge Functions, GitHub Actions |
| [nocturne-studio-web](https://github.com/kennyorlando65-prog/nocturne-studio-web) | Creative agency site with portfolio, blog, contact forms and an admin dashboard. | Next.js, React, TypeScript, Supabase |
| [orderflow](https://github.com/kennyorlando65-prog/orderflow) | Order management for small vendors, with payment links and webhook-driven fulfilment. | Node.js, Supabase, Paystack |

### On the two newest

Both are two-service deployments — a Python API and a Next.js dashboard in one repository, routed through Vercel Services — and both are honest about their own limits in the code rather than in a disclaimer.

**intelligencegrid** exists because most OSINT aggregations confuse *absence of signal* with *absence of activity*. A country with no English-language wire coverage is not a peaceful country, it is an unobserved one, and a dashboard that renders both as an empty map teaches its reader to treat blind spots as good news. So every one of the ~198 territories carries a coverage-confidence score, near-identical wire copies are grouped as syndications rather than counted as independent confirmations, and the MaritimeWatch module reports that no free global live AIS feed exists instead of approximating one. 133 backend tests and 24 frontend tests.

**crypto-anomaly-detector** shifts every rolling baseline by one observation, so the point being scored is never part of its own mean. Without that, a large move inflates the baseline and partially hides itself — look-ahead bias that makes a backtest look better than reality. There is a test asserting it. The backtest reports how many flags fired, which is a false-positive load measurement; it deliberately does not report accuracy, precision or profit, because the detectors make no prediction and any such number would be invented. 74 backend tests and 46 frontend tests.

## What I am working toward

AI/ML engineering, built on top of the systems work rather than instead of it.

I want to be direct about where I am: my shipped work today is full-stack TypeScript and Python, but it is statistics and data engineering, not machine learning. There is no model in production and no notebook on this profile yet. I would rather say that plainly than claim depth I have not earned.

The plan is to close that gap in public: a data pipeline, a model that does one useful thing, and an honest write-up of what it got wrong. When the evidence exists, it will be here.

## How I work

- Read the code before trusting the summary.
- Compute anything that touches money on the server.
- Assume every request can arrive twice.
- Write the access model before the query.
- Prefer a boring, correct solution over a clever one.

## Contact

- LinkedIn: [joshua-ubah-734856403](https://www.linkedin.com/in/joshua-ubah-734856403)
- Email: kennyorlando65@gmail.com

Open to full-stack engineering roles and to collaboration on data and ML projects.
