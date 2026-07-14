# Explore US Bikeshare Facilitation Notes

Deck: Chevron - Explore US Bikeshare Presentation v1

These notes use the current slide numbers after the interaction slides were added. If the deck is reordered later, use the slide title plus the quiz label to relocate the activity.

## Slide 11 - Basics Quiz

Slide title: Quiz: What will this code print?

Use as a quick Zoom poll after the variables/operators explanation.

Poll choices:

- A. True
- B. False
- C. It will raise an error
- D. I'm not sure yet

Correct answer: A. True

Facilitation note: Ask learners to read the code one line at a time. The expression `a == 3` is `True` because `a` stores the result of `1 + 2`.

## Slide 14 - Control Flow Quiz

Slide title: Quiz: What will this code print?

Use as a Zoom poll after the Control Flow slide.

Poll choices:

- A. City selected
- B. Chicago selected
- C. No city
- D. It will raise an error

Correct answer: A. City selected

Facilitation note: The twist is that `city` is a non-empty string, so `if city:` is already truthy. Python runs the first branch and never checks the `elif city == "Chicago"` branch. This is useful for debugging user-input checks: first ask which condition Python reaches.

## Slide 19 - Lambda Expressions Quiz

Slide title: Quiz: What will this code print?

Use as a Zoom poll after the Lambda Expressions slide.

Poll choices:

- A. [1, 2, 3]
- B. [3, 3, 3]
- C. [None, None, None]
- D. It will raise an error

Correct answer: B. [3, 3, 3]

Facilitation note: The twist is late binding. Each lambda refers to the variable `x`, not a frozen copy of its value when the lambda was created. By the time the functions run, the loop has finished and `x` is `3`.

## Slide 38 - pandas Breakout Quiz

Slide title: Quiz: Which stock is most volatile?

Use as a debrief poll after the stock-data breakout in `pandas/Statistics from Stock Data.ipynb`.

Poll choices:

- A. Google
- B. Apple
- C. Amazon
- D. Not enough information

Correct answer: C. Amazon

Facilitation note: The code compares relative volatility with `all_stocks.std() / all_stocks.mean()`. This is more useful than raw standard deviation when the stocks have very different average prices. In the supplied data, Amazon has the highest relative volatility.
