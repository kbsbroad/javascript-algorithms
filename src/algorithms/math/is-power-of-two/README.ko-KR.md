# 2의 거듭 제곱 판별

주어진 양의 정수가 2의 거듭 제곱인지 알아내는 함수를 작성하십시오.

**순수 해법**

순수 해법에서는 숫자가 `1`이되지 않는 한 `2`로 나누고, 그 때마다 나머지가 항상 `0`인 것을 확인합니다. 그렇지 않으면 숫자는 `2`의 거듭 제곱이 될 수 없습니다.

**비트단위 해법**

이진 형식의 2의 제곱은 항상 단 하나의 비트를가집니다. 유일한 예외는 부호있는 정수 (예 : `-128`의 값을 갖는 `8`비트 부호있는 정수는 `10000000`과 같습니다.)입니다.

```
1: 0001
2: 0010
4: 0100
8: 1000
```

따라서 숫자가 `0`보다 큰지 확인한 후 비트 해킹을 사용하여 하나의 비트 만 설정되어 있는지 테스트 할 수 있습니다.

```
number & (number - 1)
```

예를 들어 번호가 `8`이면 다음과 같이 보입니다.:

```
  1000
- 0001
  ----
  0111
  
  1000
& 0111
  ----
  0000    
```

## 예제

- [GeeksForGeeks](https://www.geeksforgeeks.org/program-to-find-whether-a-no-is-power-of-two/)
- [Bitwise Solution on Stanford](http://www.graphics.stanford.edu/~seander/bithacks.html#DetermineIfPowerOf2)
- [Binary number subtraction on YouTube](https://www.youtube.com/watch?v=S9LJknZTyos&t=0s&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8&index=66)
