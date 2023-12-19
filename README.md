# QArRAGgen
This is used to prepare an instruction-tuning dataset for a domain specific Llama Model. Using information from a website:
Two transformations have been done:

- **Chain of Thought Generation:**

Given an article like [**this](https://www.investopedia.com/articles/mutualfund/09/analyzing-mutual-fund-risk.asp)** The question answer generated pairs have been given below:

```markdown
1. What is the process for analyzing mutual funds?
Mutual funds are usually analyzed by weighting stocks by sector and figuring out how much management contributed to the portfolio.

2. How do you evaluate the performance of a mutual fund?
There are thousands of mutual funds in the U.S. Vanguard offers 266 funds, and its top 50 performers (by 10-year average returns) had an annual average return of 12.4%.

.... and so on
```

- **Similar Question Generation:**

Similarly, two other sets of questions are also made in order to compare how good the RAG generated question and answer pairs are

```jsx
(question, answer, [contextual similar questions],[0 shot similar questions])
```
