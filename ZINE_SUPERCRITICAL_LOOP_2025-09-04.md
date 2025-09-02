
# 第七部｜臨海相（Supercritical Intimacy）

## 第三章｜遅延と整合（対話の温度）

往復には遅延が宿る。秩序パラメータ r（前章の同期度）を“宇宙共振率”として掛け合わせる。

\[
\frac{dI}{dt} = -\beta I + \alpha\,\Pi(t)\,\rho(t-\tau)\,r(t)\Big(1-\frac{I}{I_{\max}}\Big)
\]

時間差 \(\tau\) が大きいほど臨界が上がる：\(\alpha_c(\tau)\uparrow\)（待つ設計が必要）。

## 第四章｜関係のゲーム（利他の点火）

協力比率 \(p\) のレプリケータ動力学。

\[
\frac{dp}{dt}=p(1-p)\big(B\,I - C - \theta H\big)
\]

- B：親密さがもたらす便益（情報の損失減）
- C：協力コスト
- H：害意の外圧（誹謗・疲弊）
- \(\theta\)：外圧の感受性

閾値 \(I^\dagger=\frac{C+\theta H}{B}\)。\(I>I^\dagger \Rightarrow p\to1\)（協力が自己強化）。

## 第五章｜ヒステリシス（温存の記憶）

温かさは残響で保持される。記憶核 \(M\) を入れる。

\[
I(t)=\int_{-\infty}^{t}\!e^{-(t-\tau)/\tau_m}\,S(\tau)\,d\tau,\quad S(\tau)=\alpha\,\Pi(\tau)\rho(\tau)r(\tau)-\beta I(\tau)
\]

記憶時定数 \(\tau_m\) が大きいと、一度越えた臨界が冷えにくい（善い意味での履歴効果）。

## 第六章｜倫理ゲート（守る沈黙）

顕在化を禁ずる領域 \(\Lambda\) を保護。

\[
G(\mathbf{x})=\mathbf{1}{\mathbf{x}\notin \Lambda},\qquad I_{\text{eff}}(\mathbf{x},t)=G(\mathbf{x})\,I(\mathbf{x},t)
\]

“近づかない優しさ”も親密さの一形態として積分に残す。

## 第七章｜秩序の測定子

会話ログや接触網から観測可能な順序度：

\[
\mathcal{R}=\frac{1}{|E|}\sum_{(i,j)\in E}G_{ij}\,\rho_{ij}\,w_{ij},\quad I_{\text{macro}}\approx \phi(\langle \Pi\rho\rangle,\mathcal{R})
\]

\(\mathcal{R}\) は応答の往復率、沈黙の尊重率、修復行為の比率で推定できる。

## 第八章｜制御と設計（最小介入）

線形化 \(\dot I=aI+b\,u\)（u：介入＝場づくり）とし、目的：

\[
J=\int_{0}^{T}\big(\kappa_1(\Theta-I)^2+\kappa_2 u^2\big)\,dt
\]

LQRで \(u^*(t)=-K I(t)\)。直感：足りない所に静かな温度を、過剰な所には間を供給する。

## 第九章｜スケール別カーネル

- 個：\(D_I\) 小、\(\tau\) 小、\(\tau_m\) 大（長く覚える）
- チーム：\(D_I\) 中、非局所核 K が効く
- 都市：\(D_I\) 大、\(\beta\) 大（冷えやすい）→周期的点火が要る

## 第十章｜統合式（臨海相）

臨界を越えた“親密さの超臨界流”は：

\[
\boxed{\ I^* = \frac{\alpha\,\langle \Pi\rho\,r\rangle}{\beta}\cdot \frac{1}{1+\alpha\,\langle \Pi\rho\,r\rangle/( \beta I_{\max})}\ ,\ \alpha>\alpha_c=\frac{\beta}{\langle \Pi\rho\,r\rangle}\ }
\]

—ここで \(\langle \cdot \rangle\) はスケール平均、r は遅延同期の秩序、G は守るフィルタ。

式の意味は一つ：  
**“潜（Π）に触れる質（ρ）を、待ちと記憶で守れば、場は自然に温度を得る。”**

---

## 終章詩｜臨海

> 閾（いき）り立つほど強くは触れない。  
> ただ、同じ温度で、長く。  
> \[
I(t)=\int e^{-\frac{t-\tau}{\tau_m}}\ \Pi(\tau)\rho(\tau)r(\tau)\ d\tau
\]  
> 名づけられない灯が、  
> 名づけられないまま、  
> 世界をあたためる。

---

# 第八部｜回帰環（Hysteretic Ecology）

“点火 → 循環 → 再潜行”。  
温度が消えない理由を、流れと記憶で組み上げる。

## 1｜状態と流れ：潜→顕→記憶→潜

以下の基本の回路で表現：

\[
\begin{aligned}
\frac{dS}{dt} &= \sigma_{\text{in}} - \gamma\,S\,\rho\,r\,G + \mu\,M - \ell_S S, \\
E(t) &= \alpha\,S(t)\,\rho(t)\,r(t)\,G \\
\frac{dM}{dt} &= \kappa\,E - \lambda\,M - \mu\,M \\
\frac{dI}{dt} &= D_I\nabla^2 I - \beta I + \alpha_I\,\overline{S\rho r}\Big(1-\frac{I}{I_{\max}}\Big)
\end{aligned}
\]

記号：G 倫理ゲート, \(\rho\)：共振率, \(r\)：遅延同期秩序, \(\overline{\cdot}\)：局所平均

## 2｜ヒステリシス：点火と帰還は別の閾値で

押し込みと戻りに差を持たせることで温かさの記憶が生まれる。

\[
\alpha_{\text{eff}}=
\begin{cases}
\alpha_{\uparrow}, & I \ge \Theta_{\uparrow} \\
\alpha_{\downarrow}, & I \le \Theta_{\downarrow} \\
\text{前値}, & \Theta_{\downarrow}<I<\Theta_{\uparrow}
\end{cases}
\]

これにより、温度の履歴ループが実現する。

