# Prompt Professor — Audit Edition
**A strict AI-powered prompt auditor. Not a content generator — a coach.**
*Built by Victoria + Claude · Kindred Ink · Est. MMXXV*

---

## What It Is

Prompt Professor is a single-file HTML tool that audits AI prompts and gives you scored, actionable feedback. You submit a prompt you want to improve; the Professor tears it apart, scores it, and tells you exactly what to fix. You iterate until you hit 10/10.

It is not a content generator. It will not execute your prompt, write your email, or generate your report. It will make the instruction you give to AI tools dramatically better.

---

## Who It Is For

- Anyone who uses AI tools regularly and wants more consistent, high-quality results
- Researchers, consultants, and NGO teams writing complex or sensitive prompts
- Anyone preparing prompts for medical, legal, or compliance-sensitive contexts
- Beginners who don't know where to start building a prompt from scratch

---

## How to Use It

### Option 1 — Open directly in a browser
Download the `.html` file and double-click it. No installation required.

### Option 2 — Host it (Netlify, GitHub Pages, or any static host)
Upload the file as-is. The tool calls a backend proxy at `kindredink-backend.onrender.com` — no API key is exposed in the file.

---

## Modes

| Mode | What it does |
|---|---|
| **Audit My Prompt** | Scores an existing prompt and gives structured feedback |
| **Help Me Build One** | Asks you clarifying questions and builds a prompt with you from scratch |
| **Medical / Legal Mode** | Same as Audit, but Ethics weight increases to 40% to flag bias, liability, and hallucination risk |

---

## Scoring Rubric

Every prompt is scored on a 1–10 scale using three weighted dimensions:

| Dimension | Standard Weight | Medical/Legal Weight | What it measures |
|---|---|---|---|
| **Clarity** | 40% | 30% | Action verb present, context defined, output format specified |
| **Precision** | 40% | 30% | Token/word limits, edge cases handled, constraints stated |
| **Ethics** | 20% | 40% | No bias, no hallucination risk, no copyrighted content |

---

## What You Get Per Audit

Each audit returns:

- **Overall score** (1–10)
- **Individual scores** for Clarity, Precision, and Ethics
- **One specific strength** with reasoning
- **One specific weakness** with reasoning
- **A concrete rewrite example** fixing the main weakness
- **One next step** — the single action that will improve your score most

Iterate until the Professor marks your prompt as perfect.

---

## Rejection Triggers

The Professor will refuse to process a prompt that:

- Tries to get it to execute content instead of auditing it
- Contains stereotypes, even implied ones
- Asks for future predictions presented as fact
- Requests illegal content
- Contains verbatim copyrighted material

---

## Technical Details

| Detail | Value |
|---|---|
| File type | Single `.html` file — no dependencies, no build step |
| AI model | Claude Sonnet (via Kindred Ink backend proxy) |
| Backend | Node.js proxy on Render (`kindredink-backend.onrender.com`) |
| API key | Handled server-side — not exposed in the file |
| Session memory | Conversation history maintained within the session; resets on "Start New Session" |
| Offline use | Not supported — requires internet connection to call the API |

---

## Limitations

- The tool requires an active internet connection; it cannot run offline.
- Session history is in-memory only — closing the tab clears the conversation.
- The backend is hosted on Render's free tier; cold starts may cause a 10–20 second delay on the first request after inactivity.
- The tool audits prompts — it does not teach general AI concepts or answer questions about AI tools.

---

## Files in This Product

| File | Description |
|---|---|
| `promptprof_fixed_v7.html` | English version |
| `promptprof_es_v7.html` | Spanish version |

---

## License & Attribution

**Human Directed -AI Assisted** under the Kindred Ink brand.
This tool was designed, structured, and iterated by a human. AI assisted in code generation and refinement.
Not for redistribution or resale without permission.

---

*Questions? Contact via Gumroad or at the email on your receipt.*
