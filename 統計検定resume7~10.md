# 統計検定準1級section7~10

**あとで目次をつけること**

---

## 7 極限定理、漸近理論
確率変数列$X_i$の4つの収束は、条件の強さで変わってくる
### 7.1 概収束（条件弱）
$$
\begin{align*}
p(\lim_{n\rightarrow\infty} X_n=Y)=1
\end{align*}
$$
これが成り立つのが概収束であり、例えば**大数の強法則**がある。

### 7.2 平均2乗収束(条件弱)
$$
\lim_{n\rightarrow\infty}E[(X_n-Y)^2]=0
$$
これが成り立つのが平均2乗収束であり、例えば**大数の弱法則**がある。

### 7.3 確率収束(条件中)
$$
\forall\epsilon\in\mathbb{R}_{>0}~s.t.~ \lim_{n\rightarrow\infty}p(|X_n-Y|>\epsilon)=0
$$
このとき、「$\boldsymbol{X_n\rightarrow _pY}$」と表す。
### 7.4 分布収束(条件強)
$$
\lim_{n\rightarrow\infty}F_n(x)=G(x)
$$
これが成り立つのが、分布収束といい、「$\boldsymbol{F_n\rightarrow_dG}$」と表す。

## 7.4 大数の弱法則
$X_i$が平均$\mu$、分散有限の同一の分布に独立に従うとき、その標本平均は$\mu$に**平均2乗収束**します。
### 7.5 中心極限定理
$X_i$が平均$\mu$、分散$\sigma^2$の同一の分布に従うとき、その標本平均については次の**分布収束**が成り立つ
$$
\sqrt{n}(\overline{X}_n-\mu)\rightarrow_dN(0,~\sigma^2)
$$
### 7.6 連続修正
離散分布を**中心極限定理**によって正規分布で近似するとき，区間幅を0.5だけずらして近似の精度を上げる方法。例えば，$X〜Bin(n，p)，Y〜N[np，np(1ーp)]$として，$P(a≦X≦b)$は$P(aー0.5≦Y≦b＋0.5)$でよく近似できます。次の図で，黄色いアミかけ部分$（8.5≦Y≦11.5）$と二項分布の$P(9≦X≦11)$を比べてみてください。

<img src="https://toketarou.com/wp-content/uploads/2023/10/250bb993bd1ee4bfe89292d1ab45995f.png"/>

### 7.7 連続写像定理
$X_n\rightarrow_dX$で関数$h$が連続である時、$h(X_n)\rightarrow_dh(X)$が成り立つ。
#### 7.7.1 例
$X_i$が平均$\mu$、分散$\sigma^2$の同一の分布2独立に従うとき、その標本平均について、中心極限定理によって以下の**分布収束**が成り立つ
$$
\dfrac{\sqrt{n}(\overline{X}_n-\mu)}{\sigma}\rightarrow_dN(0, 1)
$$
$f(x)=x^2$が連続関数であるから、**連続写像定理**により、次の**分布収束**が成り立つ
$$
\left(\dfrac{\sqrt{n}(\overline{X}_n-\mu)}{\sigma}\right)^2\rightarrow_d\chi^2(1)
$$

### 7.8 スルツキーの補題
$U_n→_d U，V_n→_p a$であるとき，$U_n＋V_n→_d U＋a，U_nV_n→_d aU$が成り立ちます。

### 7.9 チルダ法
次のように正規分布に分布収束する確率変数列$U_n$（サンプルサイズ$n$の標本平均$\overline{X}_n$など）を考えます。
$$
\sqrt{n}(U_n-\mu)\rightarrow_dN(0,\sigma^2)
$$
このとき，導関数が連続で$h(\mu)\neq0$を満たす関数$h$に対して次の**分布収束**が成り立ちます。

$$
\sqrt{n}\{h(U_n)-h(\mu)\}\rightarrow_dN(0, \sigma^2\{h'(\mu)\}^2)
$$














---
***github 上で編集しているときは保存をお忘れなく***































































