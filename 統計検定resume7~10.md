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
\sqrt{n}(\bar{X}_n-\mu)\rightarrow_dN(0,~\sigma^2)
$$
### 7.6 連続修正


<img src="https://toketarou.com/wp-content/uploads/2023/10/250bb993bd1ee4bfe89292d1ab45995f.png"/>
























---
***github 上で編集しているときは保存をお忘れなく***































































