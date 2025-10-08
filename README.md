
# One-file PPS Village & Household Sampler (Stratified & Unstratified) — FIX

**Fixes:**
- Persist **PPS outputs** and **Roster** in `st.session_state` so that **HH Sampling** works after Streamlit reruns.
- HH results and downloads remain visible between interactions.

**Input (single file):**
```
Woreda | Kebele | Village | Eligibility | Household Head Name [| HH_ID | Phone | Other ID]
```
**PPS base:** All | Eligible-only | Non-eligible-only

**HH Modes:** Stratified (nE/nNE) or Unstratified (n)

**Outputs:**
- `Sampled_Villages.(csv/xlsx)` with Diagnostics
- `HH_Sample.(csv/xlsx)` with HH_Summary
- Optional `Bulk_Pack.zip` (per-village CSV + PDF)
