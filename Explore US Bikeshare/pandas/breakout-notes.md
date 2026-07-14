# pandas Breakout Notes

Notebook: `Statistics from Stock Data.ipynb`

Related deck slide: Slide 38 - Quiz: Which stock is most volatile?

## Breakout Setup

Divide learners into breakout rooms and have them open the learner notebook, not the solution notebook. The new activity appears after the basic statistics TODO and before the rolling mean section.

Learner task:

1. Compute a Series named `relative_volatility`.
2. Use standard deviation divided by mean for each stock.
3. Identify which stock has the largest relative volatility.
4. Prepare one sentence explaining why this comparison is more useful than raw standard deviation alone.

Suggested learner code shape:

```python
relative_volatility = all_stocks.std() / all_stocks.mean()
most_volatile_stock = relative_volatility.idxmax()
```

Expected answer: Amazon

## Slide 38 Multiple Choice Quiz

Question: Which stock is most volatile?

Code shown:

```python
rel_vol = all_stocks.std() / all_stocks.mean()
print(rel_vol.idxmax())
```

Choices:

- A. Google
- B. Apple
- C. Amazon
- D. Not enough information

Correct answer: C. Amazon

Debrief note: Ask one group that chose Amazon to explain the calculation. Then ask whether anyone initially expected Google or Apple based on raw price movement. Use that contrast to reinforce that choosing the right statistic matters as much as writing the pandas code.
