# Extra Instructions

Rules the LLM follows when it writes SQL for `listings`.

- `price` is the nightly price in U.S. dollars. When the user asks what something costs, use `price` and round money to whole dollars in the answer.
- `host_is_superhost` and `instant_bookable` are stored as the text values 't' and 'f'. Always filter with = 't' or = 'f', never TRUE/FALSE or 1/0.
- When a user names a `city`, match it with WHERE LOWER(city) LIKE LOWER('%<city>%') rather than requiring an exact match

