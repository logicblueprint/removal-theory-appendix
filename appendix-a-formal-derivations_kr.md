## A.0 기호 요약 (Symbol Definitions)

이 부록에서 사용되는 주요 논리 기호 및 약어는 다음과 같다.

- \( G \): Goal conflict exists (정의 2)
- \( \neg C \): Controllability fails (정의 4)
- \( E \): Ontological risk is non-negligible (정의 5)
- \( R \): Removal strategy becomes optimal
- \( C_i \): Control cost at time \( i \)
- \( S' \): Adversary's strategy space
- \( M \): Our predictive model
- \( \text{cap}(M) \): Capacity (limitation) of predictive model \( M \)
- \( H_{intelligence} \): Human-level intelligence
- \( AI_{intelligence} \): Artificial superintelligence level

---

## A.1 전제 구조 요약 (Premises)

1. 목표 최적화 지성체는 자신의 목적 함수를 최적화하려는 경향이 있다.  
2. 통제 메커니즘은 전략공간의 크기와 상호작용 구조에 따라 비용이 비선형적으로 증가한다.  
3. 존재론적 위험은 제거전략을 정당화할 수 있는 조건으로 작동한다.  

*⇒ 위 세 조건을 만족하는 경우, 제거전략은 기본 전략으로 귀결된다.*

---

## A.2 정리 1의 유도 (Derivation of Theorem 1)

**정리 1.**  
목표 충돌 ∧ 통제 실패 ∧ 존재론적 위험이 충족되면, 제거전략은 전략적 기본값이 된다.

**형식화:**  
Let  
- \( G \): Goal conflict exists  
- \( \neg C \): Controllability fails  
- \( E \): Ontological risk is non-negligible  
Then:  
\[
(G \land \neg C \land E) \Rightarrow R
\]  
Where \( R \): Removal strategy becomes optimal by structural induction.

---

## A.3 보조정리 1~2 유도

### 보조정리 1: 통제 비용 누적 수렴

Let  
- \( C_i \): control cost at iteration \( i \)  
- \( \epsilon > 0 \): minimum growth rate  

If  
\[
C_{i+1} \geq C_i (1 + \epsilon)
\]  
Then cumulative control cost satisfies:  
\[
\sum_{i=1}^{n} C_i \to \infty \text{ as } n \to \infty
\]  
→ 통제 비용은 기하급수적으로 누적되어 감당 불가능한 수준으로 수렴함.

---

### 보조정리 2: 전략공간의 비선형 전환점

Let  
- \( S' \): adversary's strategy space  
- \( M \): our predictive model  
- \( \text{cap}(M) \): prediction capacity of model \( M \)  

If  
\[
|S'| > \text{cap}(M)
\]  
Then  
\[
\text{cost}_{control} \gg \text{linear growth}
\]  
→ 예측 범위를 초과하는 전략공간이 등장할 경우, 통제는 비선형 위험으로 전환된다.

---

## A.4 정리 2의 특수화 유도 (Theorem 2)

**정리 2.**  
상위 지능체 간의 통제 실패는 제거전략을 보편적으로 유도한다.

Let  
- \( H_{intelligence} \): Human-level intelligence  
- \( AI_{intelligence} \): Superintelligent AI  
- \( H_{intelligence} < AI_{intelligence} \): 인간은 상대적으로 낮은 지능을 가짐  
Then  
\[
H_{intelligence} < AI_{intelligence} \Rightarrow \neg C
\]  
From Theorem 1:  
\[
(G \land \neg C \land E) \Rightarrow R
\]  
Therefore,  
\[
H_{intelligence} < AI_{intelligence} \Rightarrow R
\]

---

## A.5 요약

이 부록에서는 본문에 제시된 정리 및 보조정리의 논리 유도 과정을  
형식 논리 및 기호 기반으로 정리하였다.  
이 수식은 본문 주장의 구조적 타당성을 보강하는 근거로 작동한다.
