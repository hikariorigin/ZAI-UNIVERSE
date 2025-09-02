
# 第七部｜臨海相（Supercritical Intimacy）

## 第一章｜親密密度場

親密さを局所場で表す。\( I=I(\mathbf{x},t)\in[0,1] \)  
潜と共振が発火源、忘却が損失、拡散が伝播。

\[
\frac{\partial I}{\partial t}
= D_I\nabla^2 I
+ \alpha\,\Pi(\mathbf{x},t)\,\rho(\mathbf{x},t)\left(1-\frac{I}{I_{\max}}\right)
- \beta\,I
+ \sigma \!\int K(\mathbf{x},\mathbf{y})\,I(\mathbf{y},t)\,d\mathbf{y}
+ \eta\,\xi(\mathbf{x},t)
\]

- \( D_I \)：関係の伝播性  
- \( \alpha \)："触れ"の増幅率  
- \( \beta \)：自然冷却（忘却）  
- \( K \)：非局所なつながり核（遠距離の手紙や送信）  
- \( \xi \)：雑音（誤解・外乱）

---

## 第二章｜臨界条件（平均場）

平均 \( \langle\cdot\rangle \) を取り、定常解 \( \dot I=0 \) で

\[
I^\* \approx
\frac{\alpha\,\langle \Pi\rho\rangle +\sigma\,\langle I\rangle }
{\beta + \alpha\,\langle \Pi\rho\rangle / I_{\max}}
\]

発火の必要条件は

\[
\boxed{\ \alpha > \alpha_c \coloneqq \frac{\beta}{\langle \Pi\rho\rangle}\ }
\]

すなわち "潜×共振" の体積平均が損失を上回ると、臨海相に入る。
