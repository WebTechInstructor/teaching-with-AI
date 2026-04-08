# Exam Prep Module Builder — Master Prompt

> Copy this prompt into Claude after uploading your source materials (slides, notes, PDFs, or study guides). Claude will read your content and generate a fully interactive, self-contained exam prep tool — no code, no installs required.

---

## How to Use This Prompt

1. **Upload your materials** — drag any slides, notes, or PDFs into Claude before pasting this prompt
2. **Paste the full prompt below** — copy everything from the horizontal rule to the end of this document
3. **Download the HTML file** Claude generates and open it in any browser

---

## The Prompt

---

### Setup Questions (Ask These First)

Before building, ask me the following questions **one at a time**:

1. Ask me to attach my source materials (slides, notes, study guides, or PDFs). Wait for me to upload them before proceeding.
2. Ask how many questions I want per section *(suggest a default of 4–5)*.
3. Ask if I want any specific topics emphasized or de-emphasized.

Once I've answered all three, build the module using the requirements below.

---

### Structure

- Divide questions into **sections that map to the major topics** in the uploaded materials
- Each section begins with a **brief concept intro** and a **row of key term chips**
- Show a **section badge** and **topic label** on every question card

---

### Question Types

- Mix **multiple choice**, **true/false**, and **select-all-that-apply** across each section
- All schemas, data tables, FD sets, code, or other reference material must be **embedded directly in the question** using a styled context box — never require the user to consult external materials

---

### Feedback

- Every question must show **detailed corrective feedback immediately** after answering — whether the answer is right or wrong
- Feedback must **explain why the correct answer is correct**, not just state it
- For wrong answers, **highlight the misconception** being corrected

---

### Tracking

- **Live dashboard** showing:
  - Correct count
  - Incorrect count
  - Running score percentage
  - Questions remaining
- **Animated progress bar**
- A **deficiency panel** that appears after the first miss and updates in real time, showing which topics have been missed and how many times

---

### Navigation

- Show **one question at a time** — do not display all questions at once
- After submitting an answer, show feedback, then a **Next Question** button to advance
- Include a **Shuffle toggle** in the header to randomize question order across all sections

---

### Remediation

- After all sections are complete, display a **summary screen** showing:
  - Final score percentage
  - Section-by-section breakdown with progress bars
  - Every missed question with: your answer, the correct answer, and the explanation
- Offer a **remediation round** that replays only the missed questions
- The remediation round must also show corrective feedback on every answer

---

### Style

- **Dark theme** with a distinctive color accent — vary it from session to session, never default to purple-on-dark or generic blue
- Use **Google Fonts** — pair a display font with a mono font for labels and code
- **Smooth slide-up animation** on each new question card
- Correct answers highlight **green**, wrong answers highlight **red**, with the correct answer always revealed

---

### Scope Discipline

- Every question must be **derivable from the uploaded source materials only**
- Do not introduce concepts, schemas, or terminology not present in the provided materials
- Do not prefix questions with phrases like *"from your slides"* or *"according to the document"* — write clean, self-contained questions

---

### Output

- Deliver a **single self-contained HTML file**
- No external dependencies, no CDN links required at runtime, no frameworks to install
- The file must open and run fully in any modern browser by double-clicking

---

## Prompt Tips — What Makes This Work

Understanding *why* this prompt produces good results helps you write your own.

| Principle | Example from this prompt | Why it matters |
|---|---|---|
| **Specify the output format exactly** | "single self-contained HTML file" | AI defaults to vague output without a concrete target |
| **Describe structure, not just content** | "Each section begins with a concept intro and key term chips" | Structural constraints produce consistent, usable layouts |
| **Define feedback behavior explicitly** | "Explain why the correct answer is correct — not just state it" | Without this, feedback is shallow ("Correct! The answer is B.") |
| **Give aesthetic constraints** | "Dark theme, Google Fonts, slide-up animation" | Vague style requests produce generic, forgettable UI |
| **Say what NOT to do** | "Never require the user to consult external materials" | Negative constraints often matter as much as positive ones |
| **Set scope boundaries** | "Only use concepts from the uploaded materials" | Prevents hallucinated content that doesn't match the source |

---

## Adapting This Prompt for Other Subjects

This prompt works for any subject with uploadable source material. Swap in your own content and adjust as needed:

- **Nursing / Medical** — upload lecture slides or a textbook chapter; emphasize clinical reasoning questions
- **History / Social Studies** — upload a reading or primary source; de-emphasize dates, emphasize causation
- **Computer Science** — upload documentation or a tutorial; request code snippet questions with embedded context boxes
- **Language Learning** — upload vocabulary lists or grammar notes; request fill-in-the-blank and translation variants
- **Certification Prep** — upload an exam outline or study guide; request questions that mirror the actual exam format

---

*Prompt authored by Thomas Wallace · Built with Claude (Anthropic)*
