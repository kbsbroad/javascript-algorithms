# 순열

순서가 중요하지 않다면, 그것은 **조합**입니다.

순서가 **중요할 때**, 그것은 **순열**입니다.

**"금고 조합은 472입니다"**. 우리는 순서에 유의해야 합니다. `724`는 동작하지 않으며, `247` 또한 마찬가지입니다. 
정확히 `4-7-2`가 되어야 합니다..

## 반복없는 순열

"배열 번호"또는 "순서"라고도하는 순열은 순서가 지정된 목록의 요소를 `S` 자체와 일대일로 다시 구성한 것입니다.

Below are the permutations of string `ABC`.

`ABC ACB BAC BCA CBA CAB`

Or for example the first three people in a running race: you can't be first and second.

**조합의 갯수**

```
n * (n-1) * (n -2) * ... * 1 = n!
```

## 반복 순열

반복이 허용될 때, 우리는 반복 순열을 가집니다. 예를 들어 아래 열쇠에서 `333`이 될 수 있습니다.

![Permutation Lock](https://www.mathsisfun.com/combinatorics/images/combination-lock.jpg)

**조합의 갯수**

```
n * n * n ... (r times) = n^r
```

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
