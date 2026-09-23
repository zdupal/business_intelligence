# Extra Instructions

Rules the LLM follows when it writes SQL for `listings`.

- `price` is the nightly price in U.S. dollars. When the user asks what something costs, use `price` and round money to whole dollars in the answer.
- `host_is_superhost` and `instant_bookable` are stored as the text values `'t'` and `'f'`, not as boolean values. Use `t` for true and `f` for false when filtering these columns.
- When averaging `review_scores_rating`, ignore rows where `review_scores_rating` is `NULL`.