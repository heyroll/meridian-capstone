# Data handling checklist — Meridian Markets engagement

Personal pre-flight checklist for this capstone project. Purpose: never let
customer or employee data reach an AI tool (ChatGPT, Claude, Copilot, or any
other), per Meridian's NDA terms in `raw/client-brief.md`.

## 1. Data classification

| Dataset | Source | AI tools (ChatGPT/Claude/Copilot/etc.) |
|---|---|---|
| POS transactions (raw, ~3 years) | POS extract | 🚫 Restricted — contains transaction-level data tied to stores/times; treat as restricted unless aggregated (see §3) |
| Loyalty membership & purchase history (~40,000 members) | Loyalty program | 🚫 Restricted — customer records, explicitly named in NDA |
| Labor scheduling & hours | HR/scheduling system | 🚫 Restricted — employee data, explicitly named in NDA |
| Store attributes (sq ft, opening date, lease terms) | Internal records | ✅ Allowed |
| Sales totals by store and week (aggregated) | Derived from POS | ✅ Allowed — explicitly named in NDA as fine to use |

If a dataset isn't on this table, default to **restricted** until you can
classify it — don't guess in the moment.

## 2. Pre-flight check — run before pasting/uploading anything into an AI tool

- [ ] Can I name exactly which dataset(s) this content came from?
- [ ] Is every one of those datasets marked ✅ Allowed in the table above?
- [ ] If it's derived/aggregated from a restricted dataset, does it pass the
      derived-data check in §3?
- [ ] Am I sending only the content needed for the task — not a wider export
      or extra columns "just in case"?
- [ ] Have I re-checked after any edit that added a join, filter, or new
      column pulled from a restricted source?

If any box is unchecked, stop and don't send it.

## 3. Derived and aggregated data

Aggregating restricted data doesn't automatically make it safe — it depends
on what the aggregate reveals.

**Generally safe:**
- Store-week (or coarser) sales totals — explicitly cleared by the client.
- Category-week totals across all stores.
- Store attribute summaries (sq ft, age, lease terms).

**Still restricted / needs judgment:**
- Any aggregate with a small `n` that could reveal an individual — e.g. a
  single loyalty member's spend in a slow week/category, or a shift with
  only one employee scheduled. Small-cell aggregates can re-identify people
  even without names attached.
- Per-member loyalty metrics (lifetime value, visit frequency, churn flags)
  at any granularity — these are still customer records.
- Per-employee labor metrics (hours, scheduling patterns) at any
  granularity — still employee data.
- Anything joining POS/loyalty/labor data together, even if summarized,
  until you've confirmed the join doesn't leak individual-level signal.

When unsure, aggregate further (widen the time window, combine categories,
raise the minimum group size) or don't send it.

## 4. Other leakage vectors

Not just the obvious file upload — these carry the same risk:

- [ ] **Screenshots** — a chart, table, or notebook screenshot can contain
      the same restricted data as the raw file.
- [ ] **Filenames / paths** pasted into a prompt (e.g. `loyalty_export.csv`)
      — usually harmless alone, but don't paste file contents alongside them.
- [ ] **Error messages / stack traces** — can include row contents, column
      values, or file previews. Read the full error before pasting; redact
      or summarize instead of pasting verbatim if unsure.
- [ ] **Code comments or variable values** — sample data in a comment,
      a hardcoded test row, or a `print()`/debug output shown to an AI tool.
- [ ] **Copy-pasted terminal output** — same risk as screenshots; check what
      a command actually printed before sharing it.

## Reference — the rule, verbatim

> "Customer records and employee data do not go into ChatGPT, Claude,
> Copilot, or any other AI tool. That includes the loyalty program data,
> the labor schedules, and any excerpts of them... Sales totals by store
> and week, and the store attributes, are fine to use with those tools."
>
> — Dana Okafor, VP of Operations, Meridian Markets (`raw/client-brief.md`)
