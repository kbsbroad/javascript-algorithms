# 배낭 문제

배낭 문제는 조합 최적화 문제입니다: 각각 무게와 가격이 있는 아이템들의 집합이 주어진다면, 집합에 들어갈 수 있는 각 아이템의 갯수를 정하십시오. 단, 총 무게는 주어진 제한 무게 이하여야 하고, 총 가격은 최대한 커야 합니다.

그것은 고정 크기 배낭에 의해 제약받는 사람이 직면 한 문제에서 그 이름을 파생시키고 그것을 가장 가치있는 항목으로 채워야합니다.

1 차원 (구속) 배낭 문제의 예 : 전체 중량을 15kg 이하로 유지하면서 금액을 최대화하기 위해 어떤 상자를 선택해야합니까?

![knapsack problem](https://upload.wikimedia.org/wikipedia/commons/f/fd/Knapsack.svg)

## 정의

### 0/1 배낭 문제

풀 수 있는 가장 일반적인 문제는 **0/1 배낭 문제**이며, 각 종류의 항목의 복사본 수를 0또는 1까지 각 아이템의 **x<sub>i</sub>** 수로 제한합니다.

`1`에서 `n`까지 번호가 매겨진 n 개의 항목 집합에서, 각각 무게 **w<sub>i</sub>** 와 가격 **v<sub>i</sub>** 이고, 최대 무게 용량은 `W`이 주어진다면,

maximize ![0/1 knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/85620037d368d2136fb3361702df6a489416931b)

subject to ![0/1 knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/dd6e7c9bca4397980976ea6d19237500ce3b8176) and ![0/1 knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/07dda71da2a630762c7b21b51ea54f86f422f951)

이다.

여기서 **x<sub>i</sub>** 는 배낭에 포함시킬 항목 `i`의 인스턴스의 수를 나타냅니다. 비공식적으로, 문제는 무게의 합이 배낭의 용량보다 작거나 같도록 배낭의 항목 값의 합을 최대화하는 것입니다.

### 경계 배낭 문제 (BKP)

**경계 배낭 문제 (BKP)** 는 각 항목 중 하나만 있다는 제한을 없애고 각 항목 종류의 복사본의 수 **x<sub>i</sub>** 를 최대 음이 아닌 정수 값 `c`로 제한합니다:

maximize ![bounded knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/85620037d368d2136fb3361702df6a489416931b)

subject to ![bounded knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/dd6e7c9bca4397980976ea6d19237500ce3b8176)
and ![bounded knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/6c8c5ac4f8247b3b8e01e89de76a1df0ea969821)

### 무한 배낭 문제 (UKP)

**무한 배낭 문제 (UKP)** 는 각 종류의 항목의 복사본 수에 상한선을 두지 않으며 위와 같이 공식화 될 수 있습니다. 단, **x<sub>i</sub>** 에 대한 유일한 제한은 음수가 아닌 정수입니다.

maximize ![unbounded knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/85620037d368d2136fb3361702df6a489416931b)

subject to ![unbounded knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/dd6e7c9bca4397980976ea6d19237500ce3b8176) 
and ![unbounded knapsack](https://wikimedia.org/api/rest_v1/media/math/render/svg/90a99710f61d5dea19e49ae5b31164d2b56b07e3)

## 레퍼런스

- [Wikipedia](https://en.wikipedia.org/wiki/Knapsack_problem)
- [0/1 Knapsack Problem on YouTube](https://www.youtube.com/watch?v=8LusJS5-AGo&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)
