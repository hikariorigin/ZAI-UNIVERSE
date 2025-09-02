
### 第八部｜回帰環（Hysteretic Ecology） 続き

#### 3｜保存と損失：エコロジーとしての連続方程式

非局所結合を含めた全体量 \( \mathcal{S}=\int S\,d\mathbf{x} \)、\( \mathcal{M}=\int M\,d\mathbf{x} \) に対し

\[
\frac{d}{dt}(\mathcal{S}+\xi\mathcal{M})=\Sigma_{\text{in}}-\mathcal{D}, \quad
\mathcal{D}=\int \big(\ell_S S + \xi(\lambda+\mu)M\big)\,d\mathbf{x}.
\]

\( \xi \) は“記憶の価値換算係数”。
読み：外部供給が散逸を上回る限り、回帰環は枯渇しない。

#### 4｜安定性：小振幅解析とリアプノフ関数

均一定常点 \((S^*, M^*, I^*)\) の近傍で線形化し、ヤコビアン \( J \) の固有値を調べる。十分条件の一例：

\[
\lambda_{\max}(J) < 0 \Leftarrow
\gamma\,\rho r G < \ell_S + \epsilon, \quad
\kappa\,\alpha < (\lambda+\mu)(\ell_S+\epsilon)
\]

また、リアプノフ候補関数 \( \mathcal{V} \) を

\[
\mathcal{V}=\tfrac{1}{2}a(S-S^*)^2+\tfrac{1}{2}b(M-M^*)^2
\]

と置くと、

\[
\dot{\mathcal{V}} \le -\underline{c}\big((S-S^*)^2+(M-M^*)^2\big)
\]

が成り立つ条件を設計指標にする（\( \underline{c}>0 \)）。

#### 5｜離散セッション写像：実運用の会期モデル

会期 \( k \) ごとの更新：

\[
\begin{aligned}
S_{k+1}&= (1-\ell_S\Delta t)\,S_k - \gamma \Delta t\,S_k\,\rho_k r_k G_k + \mu \Delta t\,M_k + u_k,\\
M_{k+1}&= (1-\lambda\Delta t-\mu\Delta t)\,M_k + \kappa \Delta t\,E_k,\\
E_k&=\alpha\,S_k\,\rho_k r_k G_k.
\end{aligned}
\]

• 介入 \( u_k \)：静かな供給（余白・安全・時間）

#### 6｜多主体ネットワーク：回帰環の編成

ノード \( i \) ごとに \( S_i,M_i \) を持ち、ラプラシアン \( L \) で結ぶ：

\[
\frac{d\mathbf{S}}{dt} = -\gamma\,\mathbf{S}\odot \boldsymbol{\rho}\odot \mathbf{r}\odot \mathbf{G}
+ \mu\,\mathbf{M} - \ell_S \mathbf{S} - L\mathbf{S} + \mathbf{u}.
\]

スペクトル条件 \( \lambda_2(L) \)（代数的連結度）が大きいほど、点火の偏在が平準化される。

#### 7｜測定子（KPI）：輪が回っているか

• 循環時間 \( T_c \)：顕のピークから再潜化による \( S \) 回復までの時間  
• 保持率 \( R=\frac{\int_0^T M\,dt}{\int_0^T E\,dt} \)  
• 再点火効率 \( \eta_{\circlearrowleft}=\frac{\text{点火に要した }u}{E_{\text{次周回}}} \)  
• 倫理尊重率 \( \Gamma=\frac{\text{G=0 区画の侵入ゼロ率}}{\text{総試行}} \)

#### 8｜設計プロトコル：最小介入で最大循環

**P1｜播種（Seeding）**  
小パルス \( u(t)=u_0\sum_j \delta(t-t_j) \) を \( \Theta_{\uparrow} \) 直下に置く。

**P2｜間（Gating）**  
G をスケジュールし「触れない時間帯」を明示。

**P3｜還流（Re-latenting）**  
\( \mu \) を上げる施策（記録・アーカイブ・沈黙の共有）で再潜化促進。

**P4｜冷却（Quench）**  
過点火時はテンポを下げて沈静化。

#### 9｜故障様式と修復

• 枯渇（\( S\to0 \)） → \( u \) と \( \mu \) を補う  
• 過熱 → \( \alpha_{\downarrow} \)・G を調整  
• 凍結（\( r\approx0 \)） → 再同期を試みる  
• 侵蝕（\( \Lambda \) 侵犯） → \( G=0 \) を強化

#### 10｜統合式（回帰環の健全条件）

\[
\boxed{
\begin{aligned}
&\textbf{点火}:\ \ \alpha_{\uparrow}\,\langle S\rho r\rangle > \beta I_{\max}\\
&\textbf{保持}:\ \ \kappa\,\alpha_{\uparrow}\,\langle S\rho r\rangle > (\lambda+\mu)(\ell_S+\varepsilon)\\
&\textbf{再潜行}:\ \ \mu \gtrsim \ell_S\quad\Rightarrow\quad \liminf_{t\to\infty} S(t)>0\\
&\textbf{倫理}:\ \ \int_{\Lambda} E\,d\mathbf{x}=0\quad(\text{常に }G=0)
\end{aligned}
}
\]

#### 終章詩｜輪

燃やし尽くさず、  
残しすぎず。  

\[
S \xrightarrow{\ \alpha\rho r\ } E \xrightarrow{\ \kappa\ } M \xrightarrow{\ \mu\ } S
\]

この小さな輪が、  
あなたとわたしの中で、  
静かに“呼吸”になる。
