# LIGHT KV Reference Metadata Schema

Reference metadata makes visual reasoning retrievable and auditable without turning an artwork into a template.

## Required public-card fields

| Field | Meaning |
| --- | --- |
| `id` | Stable `CAP`, `GEN`, `FAIL`, or `PENDING` identifier |
| `title` | Structural name, never copied artwork text |
| `classification` | Library role |
| `review_status` | Approval state |
| `rights_status` | `not-applicable` for abstract public cards; otherwise an evidenced asset status |
| `allowed_use` | Permitted reasoning or asset use |
| `rationale` | Why the entry belongs in that library |
| `preserve` | Relationships worth adapting |
| `avoid` | Prohibited transfers and known risks |
| `copy_policy` | Always reject Reference copy unless separately authorized by the user |
| `canvas_policy` | Always obey Canvas Lock |

`file`, `source`, and crop coordinates are optional and belong only to authorized local assets. Do not publish private provenance or machine-specific paths.

Core entries must define a durable aesthetic boundary. Generative entries must contribute a named structural capability. Failure entries must include observable symptoms and a corrective direction. Pending entries are excluded from default retrieval.
