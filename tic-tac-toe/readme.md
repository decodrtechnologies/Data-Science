# tic-tac-toe
## Dataset information
This database encodes the complete set of possible board configurations at the end of tic-tac-toe games, where "x" is assumed to have played first. The target concept is "win for x" (i.e., true when "x" has one of 8 possible ways to create a "three-in-a-row").

Interestingly, this raw database gives a stripped-down decision tree algorithm (e.g., ID3) fits. However, the rule-based CN2 algorithm, the simple IB1 instance-based learning algorithm, and the CITRE feature-constructing decision tree algorithm perform well on it.

Number of Instances: 958 (legal tic-tac-toe endgame boards)
Number of Attributes: 9, each corresponding to one tic-tac-toe square
Missing Attribute Values: None
Class Distribution: About 65.3% are positive (i.e., wins for "x")

## Attribute Information
V1 = top-left-square: {x,o,b}
V2 = top-middle-square: {x,o,b}
V3 = top-right-square: {x,o,b}
V4 = middle-left-square: {x,o,b}
V5 = middle-middle-square: {x,o,b}
V6 = middle-right-square: {x,o,b}
V7 = bottom-left-square: {x,o,b}
V8 = bottom-middle-square: {x,o,b}
V = bottom-right-square: {x,o,b}
V10 = Class: {positive,negative}

## Data from
https://archive.ics.uci.edu/ml/datasets/Tic-Tac-Toe+Endgame

## Libraries required
1. pandas
2. numpy
3. matplotlib
4. os
