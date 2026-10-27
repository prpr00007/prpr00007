## Hi, I'm Prabu Ramanababu

CS and Business Administration (Finance) at Northeastern University, John Martinson Honors Program, class of 2029. I build systems that run in production: trading infrastructure, computer vision pipelines, and LLM-powered tools.

**Available for co-op: January – June 2027** · software engineering, AI, and quantitative roles

[LinkedIn](https://www.linkedin.com/in/praburamanababu) · [Email](mailto:ramanababu.p@northeastern.edu)

---

### Featured projects

#### Kalshi RFQ Market-Making Bot
An automated market maker trading real capital on Kalshi, a CFTC-regulated exchange.

- Quotes both sides of multi-leg combo RFQs at ~5,000 requests/min, running 24/7 with Prometheus and Grafana monitoring
- Prices correlated parlays with a Gaussian copula fitted on 43,000+ settled windows and 100,000-path Monte Carlo
- Async event-driven engine confirms fills in ~50 ms, with layered risk controls and automatic reconciliation
- Validated through historical replay, shadow quoting, and paper trading; CI runs 67 unit tests and a replay regression

*The source is private because the bot trades live capital.*

`Python` `asyncio` `NumPy` `SQLite` `Docker` `Prometheus` `Grafana`

#### [Scriptiq](https://github.com/prpr00007/Scriptiq)
A full-stack manga localization tool. It finds the speech bubbles on a page, reads the Japanese, translates it with a vision LLM that sees the whole page, and typesets the English back into the art.

- The LLM works out who is speaking in each bubble and keeps a per-series memory of characters, glossary, and running jokes
- OpenCV bubble-shape detection fits English to the real bubble outline instead of the narrow Japanese text box
- React editor for reviewing every step: move boxes, mask art, edit lines, and translate whole chapters to a zip
- 93% text-extraction accuracy across 1,000+ pages; tested with 2 translation teams

`Python` `FastAPI` `React` `OpenCV` `manga-ocr` `EasyOCR` `Claude` `Docker`

#### [VaultOS](https://github.com/garvnn/vault-os) · BostonHacks 2025
A team hackathon project: a personal-finance dashboard that flags phishing links, automates saving, and explains transactions in plain language.

- Guard Mode scores any URL from 1 to 10 on 15+ red-flag signals (lookalike brands, punycode, shorteners, risky TLDs) without loading the page
- Smart Saver rounds up each purchase and adds a bonus when you are under budget

`Python` `FastAPI` `React` `TypeScript` `Google Gemini` `Capital One Nessie API`

---

### Tech

**Languages:** Python, Java, C++, TypeScript, JavaScript, SQL
**Frameworks:** FastAPI, React, Node.js, PyTorch, pandas, NumPy, OpenCV
**Infrastructure:** Docker, AWS, PostgreSQL, GitHub Actions, Prometheus, Grafana, Linux
