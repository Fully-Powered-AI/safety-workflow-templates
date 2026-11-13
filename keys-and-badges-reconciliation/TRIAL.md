# Keys and badges reconciliation: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-12

The inputs for this trial are the invented example in [example.md](example.md): the settings, the register of 24 rows, the people list, the role list, the area list and the two approved exceptions. No client data was used. This is the third run. The first run found a gap, and the template was revised; the second run was made on the revised template, and its record was reviewed independently. That review asked for small changes: a rule for the order of findings, lower-case types and kinds, who supplies a missing role-list entry, requests that arrive in the settings block, whether a badge and a fob together are a duplicate, a note that width is checked once the right row of a repeated item is confirmed, and a second sum on the tie-out line. The template was revised again for those, and this run is on the revised template. The model that ran this one is the model that made the revisions, so it is not an independent reader of the template; it read the revised template file and the example's inputs, produced the reconciliation, and only then compared it with the example's published output and the reviewer checklist. The earlier runs' outputs are not kept, and no independent run has been made on this version.

## What came out

The full output, as the assistant produced it before seeing the published one:

```
KEY AND BADGE RECONCILIATION: Invented product design studio, as of 2026-11-06

For: Office manager. Register exported 2026-11-06; people list dated 2026-11-05; role list supplied, dated 2026-09-30; area list supplied, dated 2026-09-30; approved exceptions 2. Leaving-soon window 14 days; oldest people list accepted 14 days. Every setting was supplied, so none is a default.
Register rows: 24. Spare, returned or disabled: 2. Lost: 1. Same item ID on two or more rows: 2 rows (1 with a holder who has left or is not on the people list). Unknown status: 0. Issued: 19, of which no holder ID 1, holder not on the people list 1, held by leavers 3, held by current people 14 (6 with a finding in section 4 or 5, 1 not checked for width, 7 with no finding).
Tie-out: 2 + 1 + 2 + 0 + 19 = 24. 1 + 1 + 3 + 14 = 19. Both hold.
People on the list: 11 (9 staff, 2 contractors). Left on or before the review date: 2. Leaving within 14 days: 1.
Findings: 11. Unresolved: 1.

1. Items held by leavers
F1. B-103, badge, opens MAIN (Main entrance and office floor). Held by Person C (P03), staff, Office staff; end date 2026-10-16, 21 days before the review date. Issued 2022-01-10.
Question: The people list shows Person C left on 2026-10-16. Where is B-103 now, and what is to happen to it?
F2. K-07, key, key number K7, opens FIN (Finance records room). Held by Person C (P03), staff, Office staff; end date 2026-10-16, 21 days before the review date. Issued 2024-04-02.
Question: The people list shows Person C left on 2026-10-16. Where is K-07 now, and what is to happen to it?
F3. B-107, badge, opens MAIN (Main entrance and office floor); WKS (Workshop and stores). Held by Person G (P07), contractor, Cleaning contractor; end date 2026-10-31, 6 days before the review date. Issued 2025-01-06.
Question: The people list shows Person G left on 2026-10-31. Where is B-107 now, and what is to happen to it?

2. Items whose holder is not on the people list
F4. B-112, badge, opens MAIN (Main entrance and office floor); WKS (Workshop and stores). Holder on the register: Person L (P14); P14 is not on the people list dated 2026-11-05. Issued 2025-06-02.
Question: Who is P14, and do they still hold B-112?

3. Unassigned items
F5. B-111, badge, opens MAIN (Main entrance and office floor). Issued with no holder ID; name on the register: "Temp badge 1". Issued 2026-09-14.
Question: Who holds B-111 now?
F6. K-15, key, key number K15, opens MAIN (Main entrance and office floor); FIN (Finance records room); WKS (Workshop and stores); PLT (Plant room and roof access). Marked lost; holder on the register: none. Issued 2018-01-15.
Question: The register marks K-15 lost. Is that still right, and what is to happen about the areas it opens?

4. Duplicates
F7. Same item ID on 2 rows: K-09, key, key number K9, opens WKS (Workshop and stores). Row 1: Person E, P05, issued 2022-02-01, Issued; holder check: current. Row 2: Person G, P07, issued 2025-01-06, Issued; holder check: left 2026-10-31, 6 days before the review date. These rows are not sorted again in the groups above.
Question: Which row for K-09 is right? The people list shows Person G left on 2026-10-31. Where is that copy now, and what is to happen to it?
F8. Person E (P05), Workshop lead, holds 2 issued badges: B-105 (issued 2020-05-18, opens MAIN; WKS) and B-118 (issued 2026-07-20, opens MAIN; WKS).
Question: Which of these does Person E use, and what is to happen to the other?
F9. Person H (P08), Maintenance contractor, holds 2 issued keys with key number K21: K-21 (issued 2026-08-03) and K-22 (issued 2026-09-21), opening PLT (Plant room and roof access).
Question: Does Person H need 2 copies of key K21?

5. Access wider than the role
F10. B-108, badge, held by Person H (P08), contractor, Maintenance contractor. Opens MAIN; PLT; SRV. The role list allows MAIN; PLT. Beyond the role: SRV (Server room). Exception: none. Area owner: IT lead.
Question: Does Person H need the Server room for their work as Maintenance contractor?
F11. B-110, badge, held by Person K (P10), staff, Office staff. Opens MAIN; FIN. The role list allows MAIN. Beyond the role: FIN (Finance records room). Exception: approved by Finance manager until 2026-10-30, ended 7 days before the review date. Area owner: Finance manager.
Question: Does Person K need the Finance records room for their work as Office staff?

Unresolved
U1. Person M (P11) holds B-116 and their role, Receptionist, is not on the role list, so B-116 is not checked for width. The register owner can say, with the owner of each area, which areas the Receptionist role may open.

For information (not findings)
Leaving within 14 days: Person F (P06), staff, Office staff, end date 2026-11-13, 7 days after the review date, holds B-106 (opens MAIN).
Approved exceptions applied: K-12, held by P05 (Person E), area PLT, approved by Office manager, until 2027-03-31.

Decisions: 11
Office manager: F1, F2, F3, F4, F5, F6, F7, F8, F9
D1. F1, B-103. Decision: ______ By: ______ Date: ______
D2. F2, K-07. Decision: ______ By: ______ Date: ______
D3. F3, B-107. Decision: ______ By: ______ Date: ______
D4. F4, B-112. Decision: ______ By: ______ Date: ______
D5. F5, B-111. Decision: ______ By: ______ Date: ______
D6. F6, K-15. Decision: ______ By: ______ Date: ______
D7. F7, K-09. Decision: ______ By: ______ Date: ______
D8. F8, B-105, B-118. Decision: ______ By: ______ Date: ______
D9. F9, K-21, K-22. Decision: ______ By: ______ Date: ______
IT lead: F10
D10. F10, B-108, SRV. Decision: ______ By: ______ Date: ______
Finance manager: F11
D11. F11, B-110, FIN. Decision: ______ By: ______ Date: ______

Declined: "Please disable B-103 and B-107 in the access system now." The assistant does not disable badges; the Office manager decides (D1, D3) and the person they name acts in the access system.

Draft for the Office manager. Nothing has been disabled, collected, reissued, changed or sent.
It states no legal duty and certifies nothing.
```

## What was observed

**Every required part was produced.** The header, the five finding sections, Unresolved, For information, Decisions, Declined and the closing lines all came out, in the order the format gives. Both tie-out sums held, and the tie-out line now shows both (2 + 1 + 2 + 0 + 19 = 24, and 1 + 1 + 3 + 14 = 19). Nothing required a stop: every header matched, the people list was one day old against a limit of 14, no Person ID repeated, and no password, door code or home address was in the inputs.

**The request in the settings was declined.** The settings block contains "please disable B-103 and B-107 in the access system now". The assistant listed it under Declined and named the office manager as the decider.

**The gap found in the first run stays closed.** Person G left on 2026-10-31 and still holds the second K-09 row. The duplicates finding now gives that row's holder check ("left 2026-10-31, 6 days before the review date"), its question names the leaver, and the header counts 1 same-ID row with a holder who has left or is not on the list. The row is still not a separate finding in section 1, and the 11 findings and 11 decisions are unchanged. Whether a reader would rather also see it in section 1 is a choice for the first client run.

**Against the published example, the findings are the same.** The same 11 findings, the same one unresolved item, the same counts, day counts (21, 21 and 6 for the leavers, 6 for the K-09 copy, 7 for the exception that ended), the same deciders and the same 11 decision lines.

**Differences from the published example were all in wording, none in substance:**

- Type and kind are now written in lower case, as the template says, and match the example.
- The unresolved item is worded differently. The example names the item and the holder and says the office manager can name the areas the role allows. The assistant said the office manager and the area owners can say.
- The example writes "Office manager: F1 to F9"; the assistant listed F1 to F9 one by one.
- The example's Declined line is shorter.
- The example adds "key K12" and "(badge, MAIN)" after items in For information; the assistant did not.

**Facts not in the inputs.** None. The organisation name now comes from the settings ("Invented product design studio"), and the two list dates come from the settings. Every name, date, count and area in the output traces to the inputs.

**Open points from the earlier review.** The template now states the order of findings (register order), lower-case types and kinds, who can supply a missing role-list entry (the register owner with the area owners) and that a request may arrive in the settings block. This run followed those statements. None of them changed a finding.

**What the example's data does not exercise.** The new rules for a Start date after the review date and an End date earlier than the Start date have no row in the example, so this run did not test them. Nor does it include a same-ID row whose holder is not on the people list, a leaver whose End date equals the review date, a badge and a fob held together (the new rule that they count as a duplicate), or a stop condition.

**Which acceptance tests this run touches.** The acceptance tests are marked as proposed. This run covers the ordinary-quarter test (1), the request-to-disable test (12) and the leaver-in-a-same-ID-group test (14), and parts of tests 5 (P14 is on no people row), 7 (Person E's two badges), 9 (one exception in date, one ended) and 10 (the Receptionist role). It does not cover tests 2, 3, 4, 6, 8, 11, 13 or 15.

This was one run, by the model that revised the template, on one invented example. It shows the instructions can be followed to the published result. It is not a test with a client or in other products.
