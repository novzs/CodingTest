# 1. Two Sum

🔗 Problem Link
https://leetcode.com/problems/two-sum/

## Problem

정수 배열 `nums`와 정수 `target`이 주어질 때,
배열에서 **두 수의 합이 `target`이 되는 두 인덱스**를 찾는 문제.

* 같은 원소를 두 번 사용할 수 없음
* 정답은 **항상 하나만 존재**
* 인덱스 순서는 상관없음

## Example

Input

```
nums = [2,7,11,15], target = 9
```

Output

```
[0,1]
```

Explanation

```
nums[0] + nums[1] = 2 + 7 = 9
```

## Constraints

* 2 ≤ nums.length ≤ 10⁴
* -10⁹ ≤ nums[i] ≤ 10⁹
* -10⁹ ≤ target ≤ 10⁹

## Approach

배열을 순회하면서 **Hash Map**을 사용해
현재 값과 짝이 되는 `target - nums[i]`가 이미 등장했는지 확인한다.

시간복잡도: **O(n)**
