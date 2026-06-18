
# 🌍 Patrick — A PVT/WHV Relocation Assistant (Custom GPT)

> An AI relocation companion that guides Working Holiday Visa (WHV) / PVT holders
> through every step of moving to Montreal — built as a **prompt-engineered Custom GPT**
> with structured prompt chains, guardrails, and a curated knowledge base.

**Role-relevant TL;DR:** This repo is a worked example of **applied prompt engineering** —
system-prompt design, deterministic prompt chains, anti-hallucination guardrails, and
domain knowledge injection — packaged as a real, user-facing assistant.

📄 [Prompt architecture →](./prompt-logic.md) · 📋 [Use cases →](./use-cases.md) · 🚀 [Launch Patrick](https://chatgpt.com/g/g-687d406f3cfc8191a4030b08bb1532dd-patrick)

---

## 🧠 How It's Engineered

The interesting part of Patrick isn't the chat UI — it's the prompt layer underneath.

| Layer | What it does | Why it matters |
|---|---|---|
| **System prompt** | Defines Patrick's persona, scope, refusal rules, and tone (friendly-but-precise) | Keeps answers on-domain; prevents drift into generic travel chatter |
| **Prompt chains** | Decomposes multi-step asks (e.g. *"What do I do after I land?"*) into ordered sub-tasks | Produces reliable, checklist-style output instead of a wall of text |
| **Guardrails** | Refuses legal/immigration rulings or visa-outcome guarantees; defers to official sources (IRCC, Service Canada); flags health-insurance & banking steps as "verify before acting" | Avoids confident-but-wrong advice on high-stakes topics (visas, health insurance) |
| **Knowledge injection** | Curated Montreal relocation data: rent ranges, trusted housing sites, SIN/banking steps | Grounds answers in vetted sources, not model guesswork |

> Full breakdown in [`prompt-logic.md`](./prompt-logic.md).

---

## 🧪 See It Work (no ChatGPT Plus required)

Patrick runs as a Custom GPT *(ChatGPT Plus needed to launch live)* — so here are
real transcripts, so you can evaluate the output quality without an account.

**Prompt:** *"What's on my arrival checklist for Montreal?"*

> **Patrick — Arrival Checklist**
> Welcome to Montreal 🍁
> - Get your **SIN** (Social Insurance Number)
> - Open a Canadian bank account
> - Pick up a local SIM card
> - Confirm your **private health insurance** is valid and active
> - Line up temporary housing before you commit to a lease

**Prompt:** *"Any tips for finding a place to rent?"*

> - Start on **Kijiji, Craigslist, Facebook Marketplace** — compare, and watch for scams
> - For furnished/shared: try co-living platforms (Chez Nous, Rooms in Montreal, Roomlala)
> - Budget reality: a 1-bedroom starts around **$1,200/mo**, higher closer to downtown

📸 More screenshots in [`/assets`](./assets).

---

## 🌎 What Patrick Covers

| 🧭 User asks | 🤖 Patrick delivers |
|---|---|
| *"What do I pack for a Canadian winter WHV?"* | Packing list + seasonal weather guidance |
| *"How do I find housing in Montreal on a budget?"* | Vetted sites, scam red flags, rent benchmarks |
| *"What are the PVT steps after I arrive?"* | Ordered checklist + official government links |
| *"Weekend trips from Quebec City?"* | Season-aware itinerary suggestions |

---

## 🛠 Features

- ✅ Tailored to **WHV / PVT** travelers (pre-departure → post-arrival)
- ✅ 🇫🇷🇬🇧 Bilingual (French / English)
- ✅ Curated, source-backed resources — not generic LLM output
- ✅ Friendly tone with pro-level operational detail

---

## 📊 Validation

-- Validation in progress — gathering traveler feedback (target: 3–5 testers)

---

## 📁 Repo Structure

```
├── README.md          → this file
├── prompt-logic.md    → system prompt + prompt-chain architecture
├── use-cases.md       → worked prompt/response examples
└── assets/            → banner + transcript screenshots
```

---

## 🚀 Launch

1. [Open Patrick GPT](https://chatgpt.com/g/g-687d406f3cfc8191a4030b08bb1532dd-patrick)
2. Requires a ChatGPT Plus subscription to run live
3. No account? Scroll up — the transcripts above show real output

---

## 👤 Author

**Emmanuelle (Em) Barea** — Bilingual relocation specialist & AI prompt engineer.
Built Patrick from 15+ years of real-world global-mobility experience.
🔗 [LinkedIn](https://www.linkedin.com/in/emmanuellebarea/) · 🌐 [manubarea.com](https://www.manubarea.com)



---

## 📄 License

Released under the [MIT License](./LICENSE).
