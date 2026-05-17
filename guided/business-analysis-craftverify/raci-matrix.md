# RACI Matrix: CraftVerify

**R** = Responsible (does the work)
**A** = Accountable (owns outcome)
**C** = Consulted (provides input)
**I** = Informed (kept in loop)

Each task has exactly one A.

| Task                              | Worker | System | CV Model | Buyer | Founders | Ops Team |
|-----------------------------------|--------|--------|----------|-------|----------|----------|
| Account signup and trade selection| R      | A      |          |       |          | I        |
| Capture and upload work sample    | R      | A      |          |       |          | I        |
| Queue sample for processing       |        | R      | I        |       |          | A        |
| Score sample against quality dims |        | I      | R        |       | A        | C        |
| Annotate and return results       | I      | R      | C        |       | A        |          |
| Choose subscription tier          | R      | I      |          |       | A        |          |
| Publish sample to portfolio       | R      | A      |          |       | I        |          |
| Index in public verified pool     |        | R      |          | I     | I        | A        |
| Search and filter worker pool     |        | A      |          | R     |          | C        |
| Hire and engage worker            | I      | I      |          | R     |          | A        |
| Rate engagement post-hire         | R      | A      |          | R     |          |          |
| Add sample to training dataset    |        | R      | C        |       | A        | I        |

## Notes

- The "Rate engagement post-hire" row has R on both Worker and Buyer because the rating is two-way and either party can initiate.
- The Ops Team is accountable for infrastructure-adjacent tasks (queue management, indexing, hire engagement coordination) while Founders are accountable for product-judgment tasks (scoring quality, annotation logic, training dataset curation).
