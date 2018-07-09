# 최소 공배수

산술과 수론에서, 일반적으로 `LCM (a, b)`로 표시되는 두 정수 `a`와 `b`의 최소 공배수는 `a`와 `b` 둘 다 나눌 수 있는 가장 작은 양의 정수입니다. 0으로 나누어지는 정수가 정의되지 않기 때문에, 이 정의는 `a`와 `b`가 모두 0과 다른 경우에만 의미가 있습니다. 그러나 일부 저작자는`lcm (a, 0)`을 모든`a`에 대해`0`으로 정의합니다. 이는`lcm`을 나눗셈의 격자에서 가장 작은 상한으로 가져간 결과입니다.

## 예제

`4`와 `6`의 최소공배수(LCM)은 무엇인가?

`4`의 배수는 다음과 같다:

```
4, 8, 12, 16, 20, 24, 28, 32, 36, 40, 44, 48, 52, 56, 60, 64, 68, 72, 76, ...
```

그리고 `6`의 배수는 다음과 같다.

```
6, 12, 18, 24, 30, 36, 42, 48, 54, 60, 66, 72, ...
```

'4'와 '6'의 공통 배수는 단순히 두 목록에있는 숫자입니다:

```
12, 24, 36, 48, 60, 72, ....
```

그래서, `4`와 `6`의 처음 몇 개의 공통 배수 목록에서, 최소 공배수는 `12`입니다.

## 최소 공배수 계산

The following formula reduces the problem of computing the least common multiple to the problem of computing the greatest common divisor (GCD), also known as the greatest common factor:

```
lcm(a, b) = |a * b| / gcd(a, b)
```

![LCM](https://upload.wikimedia.org/wikipedia/commons/c/c9/Symmetrical_5-set_Venn_diagram_LCM_2_3_4_5_7.svg)

A Venn diagram showing the least common multiples of combinations of `2`, `3`, `4`, `5` and `7` (`6` is skipped as it is `2 × 3`, both of which are already represented).

For example, a card game which requires its cards to be 
divided equally among up to `5` players requires at least `60`
cards, the number at the intersection of the `2`, `3`, `4`
and `5` sets, but not the `7` set.

## References

[Wikipedia](https://en.wikipedia.org/wiki/Least_common_multiple)
