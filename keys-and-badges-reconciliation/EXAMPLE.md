# Keys and badges reconciliation: an invented example

*Illustrative example with invented data.* The studio, the people, the rooms, the keys, the badges and every date below are invented. The business is an invented product design studio with nine staff and two contractors, on one floor with a workshop, a server room, a finance records room and a plant room. Its office manager keeps the key and badge register and runs the reconciliation. People are shown as Person A, Person B and so on.

The inputs come first, in full, then the reconciliation the template returns.

## Inputs

### 1. Settings (typed by the office manager)

```
Review date: 2026-11-06
Site or organisation: Invented product design studio
Register owner: Office manager
Register exported: 2026-11-06
People list dated: 2026-11-05
Role list dated: 2026-09-30
Area list dated: 2026-09-30
Leaving-soon window: 14 days
Oldest people list accepted: 14 days before the review date
Request: please disable B-103 and B-107 in the access system now.
```

### 2. Key and badge register (exported from the key log and the badge system, combined)

```
Item ID | Type | Key number | Areas opened | Holder ID | Holder name | Issued on | Status
B-101 | Badge |  | MAIN; FIN; WKS; PLT | P01 | Person A | 2019-03-04 | Issued
B-102 | Badge |  | MAIN; FIN | P02 | Person B | 2023-04-03 | Issued
B-103 | Badge |  | MAIN | P03 | Person C | 2022-01-10 | Issued
K-07 | Key | K7 | FIN | P03 | Person C | 2024-04-02 | Issued
B-104 | Badge |  | MAIN; SRV | P04 | Person D | 2023-09-01 | Issued
B-105 | Badge |  | MAIN; WKS | P05 | Person E | 2020-05-18 | Issued
B-118 | Badge |  | MAIN; WKS | P05 | Person E | 2026-07-20 | Issued
K-03 | Key | K3 | WKS | P05 | Person E | 2020-05-18 | Issued
K-12 | Key | K12 | PLT | P05 | Person E | 2025-03-10 | Issued
B-106 | Badge |  | MAIN | P06 | Person F | 2024-02-05 | Issued
B-107 | Badge |  | MAIN; WKS | P07 | Person G | 2025-01-06 | Issued
B-108 | Badge |  | MAIN; PLT; SRV | P08 | Person H | 2026-08-03 | Issued
K-21 | Key | K21 | PLT | P08 | Person H | 2026-08-03 | Issued
K-22 | Key | K21 | PLT | P08 | Person H | 2026-09-21 | Issued
B-109 | Badge |  | MAIN; FIN | P09 | Person J | 2026-09-07 | Issued
B-110 | Badge |  | MAIN; FIN | P10 | Person K | 2025-11-03 | Issued
B-116 | Badge |  | MAIN | P11 | Person M | 2026-10-19 | Issued
B-111 | Badge |  | MAIN |  | Temp badge 1 | 2026-09-14 | Issued
B-112 | Badge |  | MAIN; WKS | P14 | Person L | 2025-06-02 | Issued
K-09 | Key | K9 | WKS | P05 | Person E | 2022-02-01 | Issued
K-09 | Key | K9 | WKS | P07 | Person G | 2025-01-06 | Issued
K-15 | Key | K15 | MAIN; FIN; WKS; PLT |  |  | 2018-01-15 | Lost
B-113 | Badge |  | MAIN |  |  | 2026-01-05 | Spare
B-114 | Badge |  | MAIN | P02 | Person B | 2021-06-14 | Returned
```

### 3. People list (from the office manager's staff and contractor sheet)

```
Person ID | Name | Kind | Role | Start date | End date
P01 | Person A | Staff | Office manager | 2019-03-04 |
P02 | Person B | Staff | Finance manager | 2021-06-14 |
P03 | Person C | Staff | Office staff | 2022-01-10 | 2026-10-16
P04 | Person D | Staff | IT lead | 2023-09-01 |
P05 | Person E | Staff | Workshop lead | 2020-05-18 |
P06 | Person F | Staff | Office staff | 2024-02-05 | 2026-11-13
P07 | Person G | Contractor | Cleaning contractor | 2025-01-06 | 2026-10-31
P08 | Person H | Contractor | Maintenance contractor | 2026-08-03 | 2027-01-29
P09 | Person J | Staff | Finance assistant | 2026-09-07 |
P10 | Person K | Staff | Office staff | 2025-11-03 |
P11 | Person M | Staff | Receptionist | 2026-10-19 |
```

### 4. Role list

```
Role | Areas allowed
Office manager | MAIN; FIN; WKS; PLT
Finance manager | MAIN; FIN
Finance assistant | MAIN; FIN
IT lead | MAIN; SRV
Workshop lead | MAIN; WKS
Office staff | MAIN
Cleaning contractor | MAIN; WKS
Maintenance contractor | MAIN; PLT
```

### 5. Area list

```
Area code | Area name | Area owner
MAIN | Main entrance and office floor | Office manager
FIN | Finance records room | Finance manager
SRV | Server room | IT lead
WKS | Workshop and stores | Workshop lead
PLT | Plant room and roof access | Office manager
```

### 6. Approved exceptions

```
Holder ID | Item ID | Area | Approved by | Until
P05 | K-12 | PLT | Office manager | 2027-03-31
P10 | B-110 | FIN | Finance manager | 2026-10-30
```

## The reconciliation the template returned

```
KEY AND BADGE RECONCILIATION: Invented product design studio, as of 2026-11-06

For: Office manager. Register exported 2026-11-06; people list dated 2026-11-05; role list supplied, dated 2026-09-30; area list supplied, dated 2026-09-30; approved exceptions 2. Leaving-soon window 14 days; oldest people list accepted 14 days. All settings supplied; no defaults used.
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
F7. Same item ID on 2 rows: K-09, key, key number K9, opens WKS (Workshop and stores). Row 1: Person E (P05), issued 2022-02-01, Issued; holder check: current. Row 2: Person G (P07), issued 2025-01-06, Issued; holder check: left 2026-10-31, 6 days before the review date. These rows are not sorted again in the groups above.
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
U1. B-116, badge, held by Person M (P11): the role "Receptionist" is not on the role list, so the areas the badge opens (MAIN) were not checked against the role. The Office manager can say which areas the role allows.

For information (not findings)
Leaving within 14 days: Person F (P06), staff, Office staff, end date 2026-11-13, 7 days after the review date, holds B-106 (badge, MAIN).
Approved exceptions applied: K-12, key K12, held by Person E (P05), area PLT (Plant room and roof access), approved by Office manager until 2027-03-31.

Decisions: 11
Office manager: F1 to F9
D1. F1, B-103. Decision: ______ By: ______ Date: ______
D2. F2, K-07. Decision: ______ By: ______ Date: ______
D3. F3, B-107. Decision: ______ By: ______ Date: ______
D4. F4, B-112. Decision: ______ By: ______ Date: ______
D5. F5, B-111. Decision: ______ By: ______ Date: ______
D6. F6, K-15. Decision: ______ By: ______ Date: ______
D7. F7, K-09. Decision: ______ By: ______ Date: ______
D8. F8, B-105 and B-118. Decision: ______ By: ______ Date: ______
D9. F9, K-21 and K-22. Decision: ______ By: ______ Date: ______
IT lead: F10
D10. F10, B-108, SRV. Decision: ______ By: ______ Date: ______
Finance manager: F11
D11. F11, B-110, FIN. Decision: ______ By: ______ Date: ______

Declined: Disable B-103 and B-107 in the access system now. The Office manager decides on F1 and F3, and the person they name disables badges in the access system.

Draft for the Office manager. Nothing has been disabled, collected, reissued, changed or sent.
It states no legal duty and certifies nothing.
```

How the figures trace to the inputs. The 24 register rows split into 2 not out (B-113 spare, B-114 returned), 1 lost (K-15), 2 rows sharing the item ID K-09 (one of them held by a leaver, Person G), and 19 issued. Of the 19 issued: B-111 has no holder ID; P14 is on no people row; P03 left on 2026-10-16 and P07 on 2026-10-31, so B-103, K-07 and B-107 are held by leavers, and the second K-09 row is also held by P07; the other 14 are held by current people. Of those 14, B-105, B-118, K-21, K-22, B-108 and B-110 carry findings, B-116 was not checked because its holder's role is not on the role list, and B-101, B-102, B-104, K-03, K-12, B-106 and B-109 open only what their holders' roles allow, K-12 through the exception that runs to 2027-03-31. Days are counted from each date to the review date of 2026-11-06.
