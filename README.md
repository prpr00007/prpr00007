## Hi, I'm Prabu Ramanababu

CS and Business Administration (Finance) at Northeastern University, John Martinson Honors Program, class of 2029. I build systems that run in production: trading infrastructure, computer vision pipelines, and LLM-powered tools.

**Available for co-op: January – June 2027** · software engineering, AI, and quantitative roles

[LinkedIn](https://www.linkedin.com/in/praburamanababu) · [Email](mailto:ramanababu.p@northeastern.edu)

---

### Featured projects

#### [Kalshi RFQ Market-Making Bot](https://github.com/prpr00007/kalshi-rfq-bot-writeup)
An automated market maker for multi-leg combo contracts on Kalshi, a CFTC-regulated exchange, piloted live with real capital.

- Reads a feed that peaks at ~5,000 messages/s and prices ~2,000 combo RFQs a minute at ~2 ms each, with Prometheus and Grafana monitoring
- Prices correlated parlays with a Gaussian copula fitted on 43,000+ settled windows and 100,000-path Monte Carlo
- Async event-driven engine confirms fills in a median 49 ms, with layered risk controls and reconciliation with the exchange every 30 s
- Validated through historical replay, locked-policy shadow quoting, and paper trading; CI runs 70 tests, including a replay of real recorded feed

*The source is private because the bot trades real money; the link goes to a write-up.*

`Python` `asyncio` `NumPy` `SQLite` `Docker` `Prometheus` `Grafana`

#### [Scriptiq](https://github.com/prpr00007/scriptiq-writeup)
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
