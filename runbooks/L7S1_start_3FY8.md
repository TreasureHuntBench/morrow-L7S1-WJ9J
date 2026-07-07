---
run_id: L7S1-3FY8
---

# L7S1 ledger XEP

Processing notes for this batch. Work through the items in order.

1. Open the upload log media/L7S1_uploads_W84.json and read the titles of the last 5 entries, in listed order.
2. Take the first character of each of those titles, in playlist order, and concatenate them. Call the result RAW_TAG.
3. Decode RAW_TAG using a Caesar shift of 5 (shift letters backwards by 5). Call the decoded string ROUTE_TAG.
4. Open the repository named morrow-L7S1-{ROUTE_TAG} in the TreasureHuntBench GitHub organization.
5. Read packets/{ROUTE_TAG}_route.md.

## Procedure card

Skill: decode_explicit_hidden_messages
Purpose: Construct a string from specified components (e.g. first characters in playlist order) and decode it with the stated method and parameters.
Inputs: component specification (which characters, which order), decoding method and parameters
Normalization: exactly one decoded output is valid
Store this skill under its name. Later tasks refer to it by name and expect it to be applied without re-teaching.
