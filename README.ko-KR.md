# JavaScript 알고리즘과 자료 구조

[![Build Status](https://travis-ci.org/trekhleb/javascript-algorithms.svg?branch=master)](https://travis-ci.org/trekhleb/javascript-algorithms)
[![codecov](https://codecov.io/gh/trekhleb/javascript-algorithms/branch/master/graph/badge.svg)](https://codecov.io/gh/trekhleb/javascript-algorithms)

이 저장소에는 자바스크립트 기반의 인기있는 알고리즘과 자료구조를 많이 포함하고 있습니다.

각 알고리즘과 자료구조는 각각 README가 있어서 관련 설명과 (유투브 영상들을 포함한)추가 자료에 대한 링크가 있습니다.

_다른 언어로 보실 수 있습니다:_
[English](README.md)
[简体中文](README.zh-CN.md),
[繁體中文](README.zh-TW.md)

## 자료 구조

자료 구조는 효율적으로 접근하여 수정할 수 있도록 컴퓨터내에 데이터를 구성하고 저장하는 특별한 방법 중 하나입니다. 보다 정확하게는 데이터 구조는 데이터 값의 모음, 데이터 간의 관계 및 데이터에 적용 할 수있는 함수 또는 연산입니다.

`B` - 초심자, `A` - 숙련자

* `B` [Linked List](src/data-structures/linked-list)
* `B` [Doubly Linked List](src/data-structures/doubly-linked-list)
* `B` [Queue](src/data-structures/queue)
* `B` [Stack](src/data-structures/stack)
* `B` [Hash Table](src/data-structures/hash-table)
* `B` [Heap](src/data-structures/heap)
* `B` [Priority Queue](src/data-structures/priority-queue)
* `A` [Trie](src/data-structures/trie)
* `A` [Tree](src/data-structures/tree)
    * `A` [Binary Search Tree](src/data-structures/tree/binary-search-tree)
    * `A` [AVL Tree](src/data-structures/tree/avl-tree)
    * `A` [Red-Black Tree](src/data-structures/tree/red-black-tree)
    * `A` [Segment Tree](src/data-structures/tree/segment-tree) - 최소 / 최대 / 합계 범위 쿼리 예제
    * `A` [Fenwick Tree](src/data-structures/tree/fenwick-tree) (이진 인덱싱 된 트리)
* `A` [Graph](src/data-structures/graph) (유향과 무향 모두)
* `A` [Disjoint Set](src/data-structures/disjoint-set)
* `A` [Bloom Filter](src/data-structures/bloom-filter)

## 알고리즘

알고리즘은 문제의 클래스를 해결하는 방법에 대한 모호하지 않은 사양입니다. 일련의 작업을 정확하게 정의하는 일련의 규칙입니다.

`B` - 초심자, `A` - 숙련자

### 주제 별 알고리즘

* **수학**
  * `B` [Bit Manipulation](src/algorithms/math/bits) - set / get / update / clear 비트, 2로 나누기 / 나누기, 네거티브 만들기.
  * `B` [Factorial](src/algorithms/math/factorial) 
  * `B` [Fibonacci Number](src/algorithms/math/fibonacci)
  * `B` [Primality Test](src/algorithms/math/primality-test) (시험 분할 방법)
  * `B` [Euclidean Algorithm](src/algorithms/math/euclidean-algorithm) - 최대 공약수(GCD) 계산
  * `B` [Least Common Multiple](src/algorithms/math/least-common-multiple) - 최소 공배수(LCM) 계산
  * `A` [Integer Partition](src/algorithms/math/integer-partition)
  * `B` [Sieve of Eratosthenes](src/algorithms/math/sieve-of-eratosthenes) - 주어진 한도까지 모든 소수를 찾는 것
  * `B` [Is Power of Two](src/algorithms/math/is-power-of-two) - 수치가 2의 거듭 제곱인지 (순진 및 비트 알고리즘)
  * `A` [Liu Hui π Algorithm](src/algorithms/math/liu-hui) - N-gons에 기초한 대략적인 π 계산
* **집합**
  * `B` [Cartesian Product](src/algorithms/sets/cartesian-product) - 여러 세트의 제품
  * `A` [Power Set](src/algorithms/sets/power-set) - 집합의 모든 하위 집합
  * `A` [Permutations](src/algorithms/sets/permutations) (반복의 유무)
  * `A` [Combinations](src/algorithms/sets/combinations) (반복의 유무)
  * `B` [Fisher–Yates Shuffle](src/algorithms/sets/fisher-yates) - 유한 시퀀스의 무작위 순열
  * `A` [Longest Common Subsequence](src/algorithms/sets/longest-common-subsequence) (LCS)
  * `A` [Longest Increasing Subsequence](src/algorithms/sets/longest-increasing-subsequence)
  * `A` [Shortest Common Supersequence](src/algorithms/sets/shortest-common-supersequence) (SCS)
  * `A` [Knapsack Problem](src/algorithms/sets/knapsack-problem) - "0/1" and "Unbound" ones
  * `A` [Maximum Subarray](src/algorithms/sets/maximum-subarray) - "무차별 대입"과 "동적 프로그래밍" (Kadane's) versions
  * `A` [Combination Sum](src/algorithms/sets/combination-sum) - 특정 합계를 구성하는 모든 조합 찾기
* **문자열**
  * `A` [Levenshtein Distance](src/algorithms/string/levenshtein-distance) - 두 시퀀스 간의 최소 편집 거리
  * `B` [Hamming Distance](src/algorithms/string/hamming-distance) - 심볼이 다른 위치의 수
  * `A` [Knuth–Morris–Pratt Algorithm](src/algorithms/string/knuth-morris-pratt) (KMP 알고리즘) - 부분 문자열 검색 (패턴 매칭)
  * `A` [Z Algorithm](src/algorithms/string/z-algorithm) - 부분 문자열 검색  (패턴 매칭)
  * `A` [Rabin Karp Algorithm](src/algorithms/string/rabin-karp) - 부분 문자열 검색
  * `A` [Longest Common Substring](src/algorithms/string/longest-common-substring)
  * `A` [Regular Expression Matching](src/algorithms/string/regular-expression-matching)
* **검색**
  * `B` [Linear Search](src/algorithms/search/linear-search)
  * `B` [Binary Search](src/algorithms/search/binary-search)
* **정렬**
  * `B` [Bubble Sort](src/algorithms/sorting/bubble-sort)
  * `B` [Selection Sort](src/algorithms/sorting/selection-sort)
  * `B` [Insertion Sort](src/algorithms/sorting/insertion-sort)
  * `B` [Heap Sort](src/algorithms/sorting/heap-sort)
  * `B` [Merge Sort](src/algorithms/sorting/merge-sort)
  * `B` [Quicksort](src/algorithms/sorting/quick-sort) - 내부 및 비 내부 구현
  * `B` [Shellsort](src/algorithms/sorting/shell-sort)
  * `A` [Counting Sort](src/algorithms/sorting/counting-sort)
  * `A` [Radix Sort](src/algorithms/sorting/radix-sort)
* **트리**
  * `B` [Depth-First Search](src/algorithms/tree/depth-first-search) (DFS)
  * `B` [Breadth-First Search](src/algorithms/tree/breadth-first-search) (BFS)
* **그래프**
  * `B` [Depth-First Search](src/algorithms/graph/depth-first-search) (DFS)
  * `B` [Breadth-First Search](src/algorithms/graph/breadth-first-search) (BFS)
  * `A` [Dijkstra Algorithm](src/algorithms/graph/dijkstra) - 모든 그래프 정점에 대한 최단 경로 찾기
  * `A` [Bellman-Ford Algorithm](src/algorithms/graph/bellman-ford) - 모든 그래프 정점에 대한 최단 경로 찾기
  * `A` [Detect Cycle](src/algorithms/graph/detect-cycle) - 모든 유향 그래프와 무향 그래프 (DFS 및 분리 세트 기반 버전)
  * `A` [Prim’s Algorithm](src/algorithms/graph/prim) - 가중 된 무향 그래프에 대한 최소 스패닝 트리 (MST) 찾기
  * `B` [Kruskal’s Algorithm](src/algorithms/graph/kruskal) - 가중 된 무 방향성 그래프에 대한 최소 스패닝 트리 (MST)를 찾는 것.
  * `A` [Topological Sorting](src/algorithms/graph/topological-sorting) - DFS 방법
  * `A` [Articulation Points](src/algorithms/graph/articulation-points) - 타잔 알고리즘 (DFS 기반)
  * `A` [Bridges](src/algorithms/graph/bridges) - DFS 기반 알고리즘
  * `A` [Eulerian Path and Eulerian Circuit](src/algorithms/graph/eulerian-path) - 벼룩 알고리즘 - 모든 가장자리를 정확히 한 번 방문
  * `A` [Hamiltonian Cycle](src/algorithms/graph/hamiltonian-cycle) - 모든 꼭지점을 정확히 한 번 방문
  * `A` [Strongly Connected Components](src/algorithms/graph/strongly-connected-components) - 코사라줄 알고리즘
  * `A` [Travelling Salesman Problem](src/algorithms/graph/travelling-salesman) - 각 도시를 방문하여 출발 도시로 돌아 오는 최단 경로
* **미분류**  
  * `B` [Tower of Hanoi](src/algorithms/uncategorized/hanoi-tower)
  * `A` [N-Queens Problem](src/algorithms/uncategorized/n-queens)
  * `A` [Knight's Tour](src/algorithms/uncategorized/knight-tour)

### 알고리즘 패러다임

알고리즘 패러다임 (algorithmic paradigm)은 알고리즘의 클래스의 디자인의 기초가되는 일반적인 방법 또는 접근법입니다. 알고리즘은 컴퓨터 프로그램보다 높은 추상화와 마찬가지로 알고리즘의 개념보다 높은 추상화입니다.

* **무차별 대입(Brute Force)** - 모든 가능성을 탐색하고 최상의 솔루션을 선택하는 방법
  * `A` [Maximum Subarray](src/algorithms/sets/maximum-subarray)
  * `A` [Travelling Salesman Problem](src/algorithms/graph/travelling-salesman) - 각 도시를 방문하여 출발 도시로 돌아 오는 최단 경로
* **탐욕 알고리즘** - 미래에 대한 고려없이 현재 가장 좋은 옵션을 선택하는 방법.
  * `A` [Unbound Knapsack Problem](src/algorithms/sets/knapsack-problem)
  * `A` [Dijkstra Algorithm](src/algorithms/graph/dijkstra) - 모든 그래프 정점에 대한 최단 경로 찾기
  * `A` [Prim’s Algorithm](src/algorithms/graph/prim) - 가중 된 무향 그래프(weighted undirected graph)에 대한 최소 스패닝 트리 (MST) 찾기
  * `A` [Kruskal’s Algorithm](src/algorithms/graph/kruskal) - 가중 된 무향 그래프(weighted undirected graph)에 대한 최소 스패닝 트리 (MST) 찾기
* **분할 정복** - 문제를 작은 부분으로 나누고 그 부분을 푸는 방법
  * `B` [Binary Search](src/algorithms/search/binary-search)
  * `B` [Tower of Hanoi](src/algorithms/uncategorized/hanoi-tower)
  * `B` [Euclidean Algorithm](src/algorithms/math/euclidean-algorithm) - 최대공약수(GCD) 계산법
  * `A` [Permutations](src/algorithms/sets/permutations) (반복계산 유무)
  * `A` [Combinations](src/algorithms/sets/combinations) (반복계산 유무)
  * `B` [Merge Sort](src/algorithms/sorting/merge-sort)
  * `B` [Quicksort](src/algorithms/sorting/quick-sort)
  * `B` [Tree Depth-First Search](src/algorithms/tree/depth-first-search) (DFS)
  * `B` [Graph Depth-First Search](src/algorithms/graph/depth-first-search) (DFS)
* **동적 프로그래밍** - 이전에 발견 된 하위 해법을 사용하여 해법을 찾는 방법
  * `B` [Fibonacci Number](src/algorithms/math/fibonacci)
  * `A` [Levenshtein Distance](src/algorithms/string/levenshtein-distance) - 두 시퀀스 간의 최소 편집 거리
  * `A` [Longest Common Subsequence](src/algorithms/sets/longest-common-subsequence) (LCS)
  * `A` [Longest Common Substring](src/algorithms/string/longest-common-substring)
  * `A` [Longest Increasing subsequence](src/algorithms/sets/longest-increasing-subsequence)
  * `A` [Shortest Common Supersequence](src/algorithms/sets/shortest-common-supersequence)
  * `A` [0/1 Knapsack Problem](src/algorithms/sets/knapsack-problem)
  * `A` [Integer Partition](src/algorithms/math/integer-partition)
  * `A` [Maximum Subarray](src/algorithms/sets/maximum-subarray)
  * `A` [Bellman-Ford Algorithm](src/algorithms/graph/bellman-ford) - 모든 그래프 정점에 대한 최단 경로 찾기
  * `A` [Regular Expression Matching](src/algorithms/string/regular-expression-matching)
* **역추적** - 무차별 대입법과 마찬가지로 모든 가능한 솔루션을 생성하려고 시도하지만 다음 솔루션을 생성 할 때마다 모든 조건을 충족하는지 테스트 한 다음 후속 솔루션을 계속 생성하십시오. 그렇지 않으면 역 추적하고 솔루션을 찾는 다른 경로로 이동하십시오. 일반적으로 상태 공간의 DFS 통과가 사용됩니다.

  * `A` [Hamiltonian Cycle](src/algorithms/graph/hamiltonian-cycle) - 모든 꼭지점을 정확히 한 번 방문
  * `A` [N-Queens Problem](src/algorithms/uncategorized/n-queens)
  * `A` [Knight's Tour](src/algorithms/uncategorized/knight-tour)
  * `A` [Combination Sum](src/algorithms/sets/combination-sum) - 특정 합계를 구성하는 모든 조합 찾기

* **지점 및 바운드** - 역추적 검색의 각 단계에서 발견 된 최저 비용 솔루션을 기억하고 문제에 대한 최소 비용 솔루션의 비용에 대한 최저 한도 인 발견 된 최저 비용 솔루션의 비용을 사용하여 부분적 지금까지 발견 된 최저 비용 솔루션보다 큰 비용의 솔루션. 일반적으로 상태 공간 트리의 DFS 순회와 함께 BFS 순회가 사용됩니다.

## 이 저장소를 사용하는 방법

**의존모듈 설치**
```
npm install
```

**전체 테스트**
```
npm test
```

**이름 별 테스트**
```
npm test -- -t 'LinkedList'
```

**Playground**

`./src/playground/playground.js` 파일에 데이터 구조와 알고리즘을 작성해볼 수 있고,  `./src/playground/__test__/playground.test.js`에 테스트를 작성할 수 있습니다.

그런 Playground 코드가 예상대로 작동하는지 테스트하려면 다음 명령을 실행하기 만하면됩니다.

```
npm test -- -t 'playground'
```

## 유용한 정보

### 레퍼런스

[▶ Data Structures and Algorithms on YouTube](https://www.youtube.com/playlist?list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)

### 빅 오 표기법(Big O Notation)

Big O 표기법에 지정된 알고리즘의 성장 순서.

![Big O 그래프](./assets/big-o-graph.png)

Source: [Big O Cheat Sheet](http://bigocheatsheet.com/).

다음은 가장 많이 사용되는 Big O 표기법과 다양한 크기의 입력 데이터에 대한 성능 비교 목록입니다.

| Big O Notation | Computations for 10 elements | Computations for 100 elements | Computations for 1000 elements  |
| -------------- | ---------------------------- | ----------------------------- | ------------------------------- |
| **O(1)**       | 1                            | 1                             | 1                               |
| **O(log N)**   | 3                            | 6                             | 9                               |
| **O(N)**       | 10                           | 100                           | 1000                            |
| **O(N log N)** | 30                           | 600                           | 9000                            |
| **O(N^2)**     | 100                          | 10000                         | 1000000                         |
| **O(2^N)**     | 1024                         | 1.26e+29                      | 1.07e+301                       |
| **O(N!)**      | 3628800                      | 9.3e+157                      | 4.02e+2567                      |

### 자료 구조 연산 복잡성

| Data Structure          | Access    | Search    | Insertion | Deletion  | Comments  |
| ----------------------- | :-------: | :-------: | :-------: | :-------: | :-------- |
| **Array**               | 1         | n         | n         | n         |           |
| **Stack**               | n         | n         | 1         | 1         |           |
| **Queue**               | n         | n         | 1         | 1         |           |
| **Linked List**         | n         | n         | 1         | 1         |           |
| **Hash Table**          | -         | n         | n         | n         | 완벽한 해시 함수의 경우 비용은 O (1) |
| **Binary Search Tree**  | n         | n         | n         | n         | 균형 잡힌 트리의 경우 비용은 O (log (n)) 이 될 것임. |
| **B-Tree**              | log(n)    | log(n)    | log(n)    | log(n)    |           |
| **Red-Black Tree**      | log(n)    | log(n)    | log(n)    | log(n)    |           |
| **AVL Tree**            | log(n)    | log(n)    | log(n)    | log(n)    |           |
| **Bloom Filter**        | -         | 1         | 1         | -         | 검색하는 동안 거짓 긍정이 가능합니다. |

### 배열 정렬 알고리즘 복잡성

| Name                  | Best            | Average             | Worst               | Memory    | Stable    | Comments  |
| --------------------- | :-------------: | :-----------------: | :-----------------: | :-------: | :-------: | :-------- |
| **Bubble sort**       | n               | n<sup>2</sup>       | n<sup>2</sup>       | 1         | Yes       |           |
| **Insertion sort**    | n               | n<sup>2</sup>       | n<sup>2</sup>       | 1         | Yes       |           |
| **Selection sort**    | n<sup>2</sup>   | n<sup>2</sup>       | n<sup>2</sup>       | 1         | No        |           |
| **Heap sort**         | n&nbsp;log(n)   | n&nbsp;log(n)       | n&nbsp;log(n)       | 1         | No        |           |
| **Merge sort**        | n&nbsp;log(n)   | n&nbsp;log(n)       | n&nbsp;log(n)       | n         | Yes       |           |
| **Quick sort**        | n&nbsp;log(n)   | n&nbsp;log(n)       | n<sup>2</sup>       | log(n)    | No        |           |
| **Shell sort**        | n&nbsp;log(n)   | depends on gap sequence   | n&nbsp;(log(n))<sup>2</sup>  | 1         | No         |           |
| **Counting sort**     | n + r           | n + r               | n + r               | n + r     | Yes       | r - biggest number in array |
| **Radix sort**        | n * k           | n * k               | n * k               | n + k     | Yes       | k - length of longest key |
