# Portfolio Lens

Portfolio Lens is a lightweight **Jac-inspired portfolio assistant** prototype.  
It turns a simple portfolio into clear answers, allocation views, and plain-English risk summaries.

This repo is built as a **submission-ready concept package** for a small hackathon-style project. It includes:

- three polished demo mockups
- a realistic sample portfolio seeded with public market data
- a project overview
- a blog draft that can be adapted for a Jac / Jaseci community post

## Project idea

A lot of portfolio tools feel overwhelming. They show too many dashboards, metrics, and tables at once.

Portfolio Lens takes a simpler approach:

1. load a small portfolio
2. ask a question in normal language
3. get a short, grounded answer
4. see one useful chart

The goal is not to replace a professional terminal. The goal is to make portfolio questions easier to understand.

## Core features

- **Portfolio input view** for holdings, prices, shares, and weights
- **Allocation chart** that groups holdings into sectors
- **Plain-English Q&A** for common portfolio questions
- **Quick concentration checks** such as largest position, largest sector, and top-two exposure

## Demo screenshots

These lightweight SVG mockups are included directly in the repo so the demo renders cleanly on GitHub.

### 1) Portfolio input dashboard
![Portfolio input dashboard](assets/01_portfolio_input_dashboard.svg)

### 2) Allocation chart
![Allocation chart](assets/02_portfolio_allocation_chart.svg)

### 3) Chat result
![Chat result](assets/03_portfolio_chat_result.svg)

## Sample portfolio

The included demo portfolio uses five U.S. names across four sectors:

- AAPL — Apple Inc.
- MSFT — Microsoft Corp.
- JPM — JPMorgan Chase & Co.
- LLY — Eli Lilly and Co.
- PG — Procter & Gamble Co.

Sample file: `data/sample_portfolio.csv`

## What the demo shows

Using the sample portfolio, Portfolio Lens can answer questions like:

- What is my largest position?
- Which sector has the biggest weight?
- Am I too concentrated?
- Summarize this portfolio in plain English.
- What should I watch before rebalancing?

## Example result

For the current demo snapshot:

- largest holding: **AAPL**
- largest sector: **Technology**
- top two positions: **AAPL + MSFT**
- key takeaway: the portfolio is diversified across four sectors, but still leans heavily toward large-cap technology

## Why this fits Jac

This concept works well with Jac because portfolio data is naturally structured:

- a holding belongs to a sector
- a user asks for a path through that structure
- the assistant should return a precise, explainable answer

That makes the project a strong fit for a graph-oriented, AI-native workflow.

## Suggested stack

- **Jac / Jaseci** for portfolio reasoning and routing
- **Python / pandas** for table logic and aggregation
- **Simple web UI** for charts, input, and natural-language prompts

## Repo structure

```text
.
├── README.md
├── PROJECT_INTRO.md
├── BLOG_DRAFT_JACHACKS.md
├── PUBLIC_DATA_NOTES.md
├── assets/
│   ├── 01_portfolio_input_dashboard.svg
│   ├── 02_portfolio_allocation_chart.svg
│   └── 03_portfolio_chat_result.svg
└── data/
    └── sample_portfolio.csv
```

## Roadmap

- add live price updates
- support CSV upload
- generate basic diversification warnings
- add simple rebalance suggestions
- add a graph view connecting holdings, sectors, and user questions

## Status

This repo is a **prototype / concept package**.  
It is designed to help with:

- GitHub presentation
- blog writing
- demo storytelling
- submission visuals

## Short pitch

**Portfolio Lens** helps users understand a portfolio without dashboard overload.  
Instead of forcing users to dig through tables, it answers simple portfolio questions in normal language and pairs those answers with a clear allocation view.
