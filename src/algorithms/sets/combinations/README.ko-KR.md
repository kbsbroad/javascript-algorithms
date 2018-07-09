# 조합

순서가 중요하지 않다면, 그것은 **조합**입니다.

순서가 **중요할 때**, 그것은 **순열**입니다.

**"My fruit salad is a combination of apples, grapes and bananas"**
We don't care what order the fruits are in, they could also be 
"bananas, grapes and apples" or "grapes, apples and bananas", 
its the same fruit salad.

## 반복없는 조합

This is how lotteries work. The numbers are drawn one at a 
time, and if we have the lucky numbers (no matter what order) 
we win!

No Repetition: such as lottery numbers `(2,14,15,27,30,33)`

**Number of combinations**

![Formula](https://www.mathsisfun.com/combinatorics/images/combinations-no-repeat.png)

where `n` is the number of things to choose from, and we choose `r` of them,
no repetition, order doesn't matter.

It is often called "n choose r" (such as "16 choose 3"). And is also known as the Binomial Coefficient.

## 반복 조합

Repetition is Allowed: such as coins in your pocket `(5,5,5,10,10)`

Or let us say there are five flavours of ice cream: 
`banana`, `chocolate`, `lemon`, `strawberry` and `vanilla`.

We can have three scoops. How many variations will there be?

Let's use letters for the flavours: `{b, c, l, s, v}`. 
Example selections include:

- `{c, c, c}` (3 scoops of chocolate)
- `{b, l, v}` (one each of banana, lemon and vanilla)
- `{b, v, v}` (one of banana, two of vanilla)

**조합의 갯수**

![Formula](https://www.mathsisfun.com/combinatorics/images/combinations-repeat.gif)

Where `n` is the number of things to choose from, and we 
choose `r` of them. Repetition allowed, 
order doesn't matter.

## Cheat Sheets

Permutations cheat sheet

![Permutations Cheat Sheet](https://cdn-images-1.medium.com/max/2000/1*JNK-n0Pt0Vbxk0lxVpgT5A.png)

Combinations cheat sheet

![Combinations Cheat Sheet](https://cdn-images-1.medium.com/max/2000/1*7cFRn8jW4g_91YgDAbmxRQ.png)

Permutations/combinations algorithm ideas.

![Algorithms Idea](https://cdn-images-1.medium.com/max/2000/1*vLsSsZMnesCFPCYTYMbxrQ.png)

## References

- [Math Is Fun](https://www.mathsisfun.com/combinatorics/combinations-permutations.html)
- [Permutations/combinations cheat sheets](https://medium.com/@trekhleb/permutations-combinations-algorithms-cheat-sheet-68c14879aba5)
