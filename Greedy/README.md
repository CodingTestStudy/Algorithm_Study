# Greedy

---

# 1. 당장 좋은 것만 선택하는 그리디

보통 코딩 테스트에서 출제되는 그리디 알고리즘 유형의 문제는 창의력, 즉 문제를 풀기 위한 최소한의 아이디어를 떠올릴 수 있는 능력을 요구한다. 다시 말해 특정한 문제를 만났을 때 단순히 현재 상황에서 가장 좋아 보이는 것만을 선택해도 문제를 풀 수 있는지를 파악할 수 있어야 한다.<br>

'그리디'는 현재 상황에서 가장 좋아 보이는 것만을 선택하는 알고리즘이다. 현재 상황에서 가장 좋아 보이는 것만을 선택하기 때문에, 정확한 답을 도출하지 못하더라도 그럴싸한 답을 도출하는 데에 도움이 된다. 하지만 코딩 테스트에서는 대부분 '최적의 해'를 찾는 문제가 출제되기 때문에 그리디 알고리즘의 정당성을 고민하면서 문제 해결 방안을 떠올려야 한다.<br>

*keyword*

> 가장 큰 순서대로
>
> 가장 작은 순서대로

대체로 이 기준은 정렬 알고리즘을 사용했을 때 만족시킬 수 있으므로 그리디 알고리즘 문제는 자주 정렬 알고리즘과 짝을 이뤄 출제된다.



# 2. 그리디 알고리즘의 정당성

거스름돈 문제를 그리디 알고리즘으로 해결할 수 있는 이유는 가지고 있는 동전 중에서 큰 단위가 항상 작은 단위의 배수이므로 작은 단위의 동전들을 종합해 다른 해가 나올 수 없기 때문이다. 대부분의 그리디 알고리즘 문제에서는 이처럼 문제 풀이를 위한 최소한의 아이디어를 떠올리고 이것이 정당한지 검토할 수 있어야 답을 도출할 수 있다.<br>

*keyword*<br>

문제 --> (바로 문제 유형을 해결하기 어렵다면?) --> 완전 탐색 --> 그리디 알고리즘 --> 다이나믹 프로그래밍 or 그래프 알고리즘



# 3. Discussion
## 만들 수 없는 금액 문제
현재 상태를 '1부터 target - 1까지의 모든 금액을 만들 수 있는 상태'라고 하자.<br>
이때 매번 target인 금액도 만들 수 있는지(현재 확인하는 동전의 단위가 target 이하인지) 체크하는 아이디어로 문제를 해결할 수 있다.