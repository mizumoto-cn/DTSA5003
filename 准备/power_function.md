# Power Function

## Power Function Explained

### What is a Power Function?

In the context of hypothesis testing, the **power function** \(\gamma(\theta)\) is a function that describes the probability of correctly rejecting the null hypothesis \(H_0\) given a particular value of the parameter \(\theta\). This function helps us understand how well our test performs across different possible values of \(\theta\).

Formally, for a given test with a parameter \(\theta\), the power function \(\gamma(\theta)\) is defined as:

\[
\gamma(\theta) = P(\text{Reject } H_0 \mid \theta)
\]

Where:

- \(\gamma(\theta)\) is the power at the value \(\theta\).
- \(P(\text{Reject } H_0 \mid \theta)\) is the probability of rejecting the null hypothesis given that the true parameter value is \(\theta\).

### Key Concepts Related to Power Function

1. **Significance Level (\(\alpha\))**:
   - The significance level, \(\alpha\), is the probability of rejecting the null hypothesis when it is actually true. In other words, it's the probability of making a Type I error.
   - For values of \(\theta\) that fall within the null hypothesis (\(H_0\)), the power function \(\gamma(\theta)\) should not exceed \(\alpha\). Therefore, the maximum value of \(\gamma(\theta)\) within \(H_0\) is typically \(\alpha\).

2. **Type II Error and Power**:
   - A **Type II error** occurs when the test fails to reject \(H_0\) when \(H_1\) (the alternative hypothesis) is true.
   - The power of a test, \(1 - \beta(\theta)\), where \(\beta(\theta)\) is the probability of a Type II error, represents the probability of correctly rejecting \(H_0\) when a specific alternative is true.

3. **Behavior of the Power Function**:
   - **Within \(H_0\)**: \(\gamma(\theta)\) is at most \(\alpha\), reflecting the fact that the test should rarely reject \(H_0\) when it is true.
   - **Within \(H_1\)**: \(\gamma(\theta)\) increases as \(\theta\) moves further away from the null hypothesis region, indicating a higher probability of rejecting \(H_0\) when the alternative hypothesis is true.

4. **Range of the Power Function**:
   - The power function values lie between 0 and 1 (inclusive), since it represents a probability.

### Example to Illustrate

Imagine a test designed to determine whether a coin is fair (i.e., whether the probability of heads, \(\theta\), is 0.5).

- **Null Hypothesis (\(H_0\))**: \(\theta = 0.5\)
- **Alternative Hypothesis (\(H_1\))**: \(\theta \neq 0.5\)

For different values of \(\theta\), the power function \(\gamma(\theta)\) will tell us the probability that the test correctly rejects \(H_0\):

- If \(\theta = 0.5\), \(\gamma(0.5)\) would be around \(\alpha\) (since under \(H_0\), we should only reject it with a probability \(\alpha\)).
- As \(\theta\) moves away from 0.5 (e.g., \(\theta = 0.6\) or \(\theta = 0.4\)), the power \(\gamma(\theta)\) increases, indicating that the test becomes more likely to correctly reject \(H_0\).

## Summary

- The power function \(\gamma(\theta)\) measures the effectiveness of a hypothesis test across different values of \(\theta\).
- It helps in understanding both the likelihood of making correct decisions and the risks of making errors (Type I and Type II).
- The values of \(\gamma(\theta)\) range from 0 to 1, with the function reflecting the test's power against alternatives to the null hypothesis.

This function is a fundamental concept in hypothesis testing, providing insights into the test's sensitivity and robustness.

## 功效函数解释

### 什么是功效函数？

在假设检验中，**功效函数** \(\gamma(\theta)\) 是一个描述在给定参数 \(\theta\) 的情况下，正确拒绝原假设 \(H_0\) 的概率的函数。这个函数帮助我们理解在不同的 \(\theta\) 值下，我们的检验性能如何。

形式上，对于一个给定的参数 \(\theta\) 的检验，功效函数 \(\gamma(\theta)\) 定义为：

\[
\gamma(\theta) = P(\text{Reject } H_0 \mid \theta)
\]

其中：

- \(\gamma(\theta)\) 是在 \(\theta\) 值下的功效。
- \(P(\text{Reject } H_0 \mid \theta)\) 是在真实参数值为 \(\theta\) 时拒绝原假设的概率。

### 功效函数相关的关键概念

1. **显著性水平 (\(\alpha\))**:
   - 显著性水平 \(\alpha\) 是指当原假设 \(H_0\) 为真时，拒绝 \(H_0\) 的概率。换句话说，这是犯第一类错误的概率。
   - 对于属于 \(H_0\) 的 \(\theta\) 值，功效函数 \(\gamma(\theta)\) 不应超过 \(\alpha\)。因此，在 \(H_0\) 范围内，\(\gamma(\theta)\) 的最大值通常为 \(\alpha\)。

2. **第二类错误与功效**:
   - **第二类错误** 指的是当 \(H_1\)（备择假设）为真时，检验没有拒绝 \(H_0\)。
   - 检验的功效 \(1 - \beta(\theta)\)，其中 \(\beta(\theta)\) 是第二类错误的概率，表示当特定备择假设为真时，正确拒绝 \(H_0\) 的概率。

3. **功效函数的行为**:
   - **在 \(H_0\) 内**：\(\gamma(\theta)\) 最多为 \(\alpha\)，反映出当 \(H_0\) 为真时，检验应该很少拒绝 \(H_0\)。
   - **在 \(H_1\) 内**：当 \(\theta\) 远离原假设区域时，\(\gamma(\theta)\) 增加，表明当备择假设为真时，拒绝 \(H_0\) 的概率更高。

4. **功效函数的范围**:
   - 功效函数的值在 0 到 1 之间（包括0和1），因为它表示的是概率。

### 例子说明

假设我们设计了一个检验来判断一枚硬币是否公平（即硬币正面朝上的概率 \(\theta\) 是否为0.5）。

- **原假设 (\(H_0\))**：\(\theta = 0.5\)
- **备择假设 (\(H_1\))**：\(\theta \neq 0.5\)

对于不同的 \(\theta\) 值，功效函数 \(\gamma(\theta)\) 会告诉我们检验正确拒绝 \(H_0\) 的概率：

- 如果 \(\theta = 0.5\)，则 \(\gamma(0.5)\) 大约为 \(\alpha\)（因为在 \(H_0\) 下，我们只有概率为 \(\alpha\) 才会拒绝它）。
- 当 \(\theta\) 偏离0.5（例如 \(\theta = 0.6\) 或 \(\theta = 0.4\)）时，功效 \(\gamma(\theta)\) 增加，表明检验更可能正确拒绝 \(H_0\)。

## 总结

- 功效函数 \(\gamma(\theta)\) 衡量了假设检验在不同 \(\theta\) 值下的有效性。
- 它帮助我们理解在做出正确决策的可能性以及犯错误（第一类和第二类错误）的风险。
- \(\gamma(\theta)\) 的值范围是从0到1，反映了检验对备择假设的敏感性和稳健性。

功效函数是假设检验中的一个基本概念，它为我们提供了关于检验灵敏度和可靠性的重要信息。
