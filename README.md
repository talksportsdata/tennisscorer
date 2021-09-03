# Tennisscorer
> A Python library that allows you to track you tennis score.


## Install

`pip install tennisscorer`

## How to use

Use the `SetTracker`.

```python
scores = random.choices(population=[True, False], k=20)
final_set = SetTracker(12, 12, final_point=12)

for score in scores:
    final_set.increase(score)
    print(final_set)
    if final_set.finished:
        print('Game is over.')
        print(final_set.is_winner_home)
        break
```
