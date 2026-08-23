# Anime Data Model

Each record represents one anime movie.

| Field | Type | Purpose |
|---|---|---|
| `id` | string | Stable unique identifier |
| `title` | string | Display title |
| `type` | string | Media type; currently `movie` |
| `year` | integer | Release year |
| `genres` | string[] | Primary genres |
| `score` | number | Rating from 0 to 10 |
| `duration_minutes` | integer | Runtime in minutes |
| `language` | string | Primary language |
| `tags` | string[] | Recommendation/search keywords |

## Design goals

- Keep records platform-neutral.
- Use predictable field names for frontend applications.
- Keep the schema strict enough for validation.
- Allow recommendation systems to use genres, tags, score, year, and runtime.
