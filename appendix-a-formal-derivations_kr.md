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
- \( H_{intelligence} < AI_{intelligence} \): human is cognitively inferior  
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
