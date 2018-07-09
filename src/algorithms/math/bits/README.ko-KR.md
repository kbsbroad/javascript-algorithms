# Bit Manipulation

#### 비트 가져 오기

이 메서드는 해당 비트를 0 번째 위치로 이동합니다. 그런 다음 '0001`과 같은 비트 패턴을 가진 AND 연산을 수행합니다. 해당 번호를 제외한 원래 번호의 모든 비트가 지워집니다. 관련 비트가 1이면 결과는 '1'이고, 그렇지 않으면 결과는 '0'입니다.

> 자세한 것은`getBit` 함수를 참고하십시오.

#### 비트 설정

이 방법은`bitPosition` 비트에 의해`1`을 시프트하여`00100`과 같은 값을 생성합니다. 그런 다음 특정 비트를 '1'로 설정하는 'OR'연산을 수행하지만 숫자의 다른 비트에는 영향을 미치지 않습니다.

> 자세한 것은`setBit` 함수를 참고하십시오.

#### 비트 지우기

이 방법은`bitPosition` 비트에 의해`1`을 시프트하여`00100`과 같은 값을 생성합니다. 그런 다음 이 마스크를 반전하여 '11011'과 같은 숫자를 얻습니다. 그런 다음 AND와 연산이 숫자와 마스크에 모두 적용됩니다. 이 작업은 비트를 설정 해제합니다.

> 자세한 것은`clearBit` 함수를 참고하십시오.

#### 비트 갱신

이 방법은 "비트 지우기"및 "비트 설정"방법의 조합입니다.

> 자세한 것은`updateBit` 함수를 참고하십시오.

#### 2로 곱하기

이 방법은 원래 숫자를 1 비트 왼쪽으로 이동합니다. 따라서 모든 이진수 구성 요소 (2의 제곱)에 2가 곱해 지므로 숫자 자체에 2가 곱 해집니다.

```
Before the shift
Number: 0b0101 = 5
Powers of two: 0 + 2^2 + 0 + 2^0 

After the shift
Number: 0b1010 = 10
Powers of two: 2^3 + 0 + 2^1 + 0 
```

> 자세한 것은`multiplyByTwo` 함수를 참고하십시오.

#### 2로 나누기

이 방법은 원래 숫자를 오른쪽으로 1 비트 씩 이동합니다. 따라서 모든 2 진수 구성 요소 (2의 제곱)는 2로 나누어지고 따라서 숫자 자체는 나머지없이 2로 나눕니다.

```
Before the shift
Number: 0b0101 = 5
Powers of two: 0 + 2^2 + 0 + 2^0 

After the shift
Number: 0b0010 = 2
Powers of two: 0 + 0 + 2^1 + 0 
```

> 자세한 내용은`divideByTwo` 함수를 참고하십시오.

#### 부호 변경

이 메서드는 양수가 음수가 되도록합니다. 이렇게 하려면 "Two's Complement" 접근법을 사용합니다. 이 방법은 숫자의 모든 비트를 반전시키고 1을 더하는 방식으로 수행합니다.

```
1101 -3
1110 -2
1111 -1
0000  0
0001  1
0010  2
0011  3
``` 

> 자세한 내용은`switchSign` 함수를 참고하십시오.

## 레퍼런스

- [Bit Manipulation on YouTube](https://www.youtube.com/watch?v=NLKQEOgBAnw&t=0s&index=28&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)
- [Negative Numbers in binary on YouTube](https://www.youtube.com/watch?v=4qH4unVtJkE&t=0s&index=30&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)
- [Bit Hacks on stanford.edu](https://graphics.stanford.edu/~seander/bithacks.html)
