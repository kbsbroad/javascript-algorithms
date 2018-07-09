# Levenshtein 거리

Levenshtein 거리는 두 시퀀스 간의 차이를 측정하기위한 문자열 메트릭입니다. 비공식적으로, 두 단어 사이의 Levenshtein 거리는 한 단어를 다른 단어로 바꾸는 데 필요한 최소 한 문자 편집 (삽입, 삭제 또는 대체) 횟수입니다.

## 정의

수학적으로 두 문자열 사이의 Levenshtein 거리
`a`와`b` (각각 길이`| a |`와`| b |`)는 다음과 같이 의해 주어진다.

![Levenshtein](https://wikimedia.org/api/rest_v1/media/math/render/svg/4cf357d8f2135035207088d2c7b890fb4b64e410)

where

![Levenshtein](https://wikimedia.org/api/rest_v1/media/math/render/svg/f0a48ecfc9852c042382fdc33c19e11a16948e85)

where 

![Levenshtein](https://wikimedia.org/api/rest_v1/media/math/render/svg/52512ede08444b13838c570ba4a3fc71d54dbce9)

is the indicator function equal to `0` when

![Levenshtein](https://wikimedia.org/api/rest_v1/media/math/render/svg/231fda9ee578f0328c5ca28088d01928bb0aaaec)

and equal to 1 otherwise, and

![Levenshtein](https://wikimedia.org/api/rest_v1/media/math/render/svg/bdc0315678caad28648aafedb6ebafb16bd1655c)

is the distance between the first `i` characters of `a` and the first `j` characters of `b`.

Note that the first element in the minimum corresponds to deletion (from `a` to `b`), the second to insertion and the third to match or mismatch, depending on whether the respective symbols are the same.

## 예제

For example, the Levenshtein distance between `kitten` and `sitting` is `3`, since the following three edits change one into the other, and there is no way to do it with fewer than three edits:

1. **k**itten → **s**itten (substitution of "s" for "k")
2. sitt**e**n → sitt**i**n (substitution of "i" for "e")
3. sittin → sittin**g** (insertion of "g" at the end).

## 응용 분야

여기에는 맞춤법 검사기, 광학 문자 인식 교정 시스템, 퍼지 문자열 검색 및 번역 메모리를 기반으로 자연어 번역을 지원하는 소프트웨어와 같은 다양한 응용 프로그램이 있습니다.

## 동적 프로그래밍 접근법 설명

`ME`와 `MY` 사이의 최소 편집 거리를 찾는 간단한 예제를 살펴 보겠습니다. 직관적으로 당신은 이미 최소 편집 거리가 `1` 연산이고 이 연산을 이미 알고 있습니다. 그리고 그것은`E`를 `Y`로 대체하는 것입니다. 그러나 `Saturday`를 `Sunday`로 변환하는 것과 같은 보다 복잡한 예제를 수행 할 수 있도록 알고리즘의 형식으로 공식화합시다.

To apply the mathematical formula mentioned above to `ME → MY` transformation 
we need to know minimum edit distances of `ME → M`, `M → MY` and `M → M` transformations
in prior. Then we will need to pick the minimum one and add _one_ operation to 
transform last letters `E → Y`. So minimum edit distance of `ME → MY` transformation 
is being calculated based on three previously possible transformations.

To explain this further let’s draw the following matrix:

![Levenshtein Matrix](https://cdn-images-1.medium.com/max/1600/1*2d46ug_PL5LfeqztckoYGw.jpeg)

- Cell `(0:1)` contains red number 1. It means that we need 1 operation to 
transform `M` to an empty string. And it is by deleting `M`. This is why this number is red.
- Cell `(0:2)` contains red number 2. It means that we need 2 operations 
to transform `ME` to an empty string. And it is by deleting `E` and `M`.
- Cell `(1:0)` contains green number 1. It means that we need 1 operation 
to transform an empty string to `M`. And it is by inserting `M`. This is why this number is green.
- Cell `(2:0)` contains green number 2. It means that we need 2 operations 
to transform an empty string to `MY`. And it is by inserting `Y` and  `M`.
- Cell `(1:1)` contains number 0. It means that it costs nothing 
to transform `M` into `M`.
- Cell `(1:2)` contains red number 1. It means that we need 1 operation 
to transform `ME` to `M`. And it is be deleting `E`.
- And so on...

This looks easy for such small matrix as ours (it is only `3x3`). But here you
may find basic concepts that may be applied to calculate all those numbers for
bigger matrices (let’s say `9x7` one, for `Saturday → Sunday` transformation).

According to the formula you only need three adjacent cells `(i-1:j)`, `(i-1:j-1)`, and `(i:j-1)` to
calculate the number for current cell `(i:j)`. All we need to do is to find the 
minimum of those three cells and then add `1` in case if we have different 
letters in `i`'s row and `j`'s column.

You may clearly see the recursive nature of the problem.

![Levenshtein Matrix](https://cdn-images-1.medium.com/max/2000/1*JdHQ5TeKiDlE-iKK1s_2vw.jpeg)

Let's draw a decision graph for this problem.

![Minimum Edit Distance Decision Graph](https://cdn-images-1.medium.com/max/1600/1*SGwYUpXH9H1xUeTvJk0e7Q.jpeg)

You may see a number of overlapping sub-problems on the picture that are marked 
with red. Also there is no way to reduce the number of operations and make it 
less then a minimum of those three adjacent cells from the formula. 

Also you may notice that each cell number in the matrix is being calculated 
based on previous ones. Thus the tabulation technique (filling the cache in 
bottom-up direction) is being applied here.

Applying this principles further we may solve more complicated cases like 
with `Saturday → Sunday` transformation.

![Levenshtein distance](https://cdn-images-1.medium.com/max/1600/1*fPEHiImYLKxSTUhrGbYq3g.jpeg)

## References

- [Wikipedia](https://en.wikipedia.org/wiki/Levenshtein_distance)
- [YouTube](https://www.youtube.com/watch?v=We3YDTzNXEk&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)
- [ITNext](https://itnext.io/dynamic-programming-vs-divide-and-conquer-2fea680becbe)
