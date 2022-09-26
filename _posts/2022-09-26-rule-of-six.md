---
title: Rule of Six
src: https://davidamos.dev/the-rule-of-six
categories: [Programming]
tags: [opinionated, principles, extra-short]
---

A line of code should do <6 things.

- :six: human short-term & working memory can only cope with [upto 6 pieces of info](https://en.m.wikipedia.org/wiki/The_Magical_Number_Seven,_Plus_or_Minus_Two) simultaneously

```python
# bad
map(lambda x: x.split('=')[1], s.split('?')[1].split('&')[-3:])
```

```python
# good
url_query_string = s.split('?')[1]
query_params = url_query_string.split('&')[-3:]
map(lambda x: x.split('=')[1], query_params)
```

## personal opinion

:thinking: The article begins by implying `x, y = 2, 7` is bad. I disagree. I am against blanket-banning legitimate language features. Such bans miss the point. The point is to minimise time-to-comprehend. Everything needs to be considered on a case-by-case basis.

Highly human-readable, brilliant inlining of a single-use `class TimeWindow(start, stop)`:

```python
start, end = 2, 7 # time window in hours
max_retries = 1   # unrelated to above, so separate line
```
