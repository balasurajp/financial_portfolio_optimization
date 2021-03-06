---
layout: default
---

<!-- 
Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.PNG)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.PNG)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
 -->
 
 
# Introduction

Portfolio Optimization is a fundamental process in financial planning which involves constant redistribution of the investment into various financial products with an primary objective of maximal profits with minimal risks. In mathematical terms, it's a process involving continuous analysis of financial asset's data to make optimal sequential decisions i.e a classical prospective problem for reinforcement learning and deep learning. As financial markets evolves continuously over time without constant dynamics and the information regarding the financial products is diverse in many aspects, a robust and adaptive financial system with generic implementation to different financial markets such as stocks, forex and cryptos is essential.

# Research Objectives

In this project, all the frameworks has a fundamental aim of maximising forecasted profits and also minimising calculated risks through optimal asset allocation for a given fixed time horizon. For experimental purposes, any financial market is constructed using relavant asset information with an assumption that it has sufficient liquidity so that any order gets transacted with negligible market impact. This market system with operational dynamics is casted into a simulated environment for all purposes. For portfolio allocation, we consider adaptive autonomous agent that gathers all required information from market to make decisions and to improve its trading strategy through several interacting experiences.
 
# Simulated Environment

Let's consider the number of financial assets that agent would invest is \\( N \\). For simplicity, we assume our total investment capital is 1.0 unit base asset at initial timeperiod. Now, let's define _relative price vector of close-open prices_ and _portfolio weight vector_ where \\( \frac{v_{i, t}^{close}}{v_{i, t}^{open}} \\) is _relative price_ and \\( w_{i,t} \\) is the _fraction of capital_ of asset \\(i\\) at timeperiod \\(t\\). 
  
  $$ y_t=[1, \frac{v_{1,t}^{close}}{v_{1,t}^{open}}, \frac{v_{2,t}^{close}}{v_{2,t}^{open}},\cdots,\frac{v_{N,t}^{close}}{v_{N,t}^{open}}] $$

  $$ w_t=[w_{0,t}, w_{1, t}, \cdots, w_{N, t}] $$

  $$ \sum_{i=0}^{N}w_{i, t}=1 $$

In any fixed horizon simulation, the total capital value after timestamp \\(T\\) while considering the transaction cost factor \\( \mu \\) is

  $$ p_T=\prod_{t=1}^{T}(1-\mu\sum{|\frac{y_t \odot w_{t-1}}{y_t \cdot w_{t-1}} - w_{t}|}) y_t\cdot w_{t-1} $$

# Proposed Methodology

The trading agent with desired objective is achieved through different formulations such as

- **Reinforcement learning formulation**: The interaction between the simulated environment and the trading agent can be formulated into Markov Decision Process with appropriate state, action and reward mechanisms. This MDP formulation can be solved using various model-free reinforcement algorithms such as DQN, DDPG, PPO, SAC etc...

- **Deep learning formulation**: Using the appropriate assumptions, this problem can be formulated into supervised learning framework, where state-action-reward can be viewed as input-output-objective. This is typically one-way to model this problem and there exists several ways in which this problem can be solved using deep learning.

_Note: There is only limited amount of information and no project-code here due to TCS confidentiality and Intellectual property rights_

# Conclusion 

To conclude, there is alot of scope for advancements using machine learning and reinforcement learning in the problem of wealth management in the domain of Quantitative finance. 

# References
1. https://arxiv.org/abs/1706.10059
2. http://www-scf.usc.edu/~zhan527/post/cs599/
