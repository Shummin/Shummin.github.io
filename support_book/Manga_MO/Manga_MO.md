# マンガでわかる数理最適化　（オーム社）
## はじめに
本サイトは，オーム社より出版された「<a href="https://www.ohmsha.co.jp/book/9784274232008/">マンガでわかる数理最適化</a>」のサポートページです．
わかりやすさを重視して厳密性を欠いてしまい，専門的には語弊が生じるようなことや，誤植等が多々あると思います．
このサポートページでは，それらの問題点を解消したいと思います．

ここに書かれていることの他に，指摘や誤植の発見等がありましたら snakayama<@>uec.ac.jp に連絡してください．


## 正誤表
|該当ページ|該当箇所| 誤 | 正 | 補足 |
| :--- | :--- | :--- | :--- | :--- |
| p.54 | １変数のグラフの中 | $z = f(x)$ | $y = f(x)$ | |
| p.60 | (1.2) |　-　| (1.1)と合わせるならmaxとminの順番が逆です | |
| p.73 | 二つ目の制約条件の中 |　$a_{0+1,1}$等の添字　| 補足参照 |[添え字の訂正](#p73) |
| p.87 | 最後の行 | 最適 **解** が一致 | 最適 **値** が一致 | |
| p.89 | 双対定理の中 | 最適 **解** が一致する | 最適 **値** が一致 | [強双対定理の補足](#strong_dual) |
| p.95 | 3.の最適解 | $(y_1,y_2)=(1,3)$ | $(y_1,y_2)=(100,300)$ | |
| p.193 | $Ax$の最後の成分 | \sum_{i=1}^n a_{2,i} x_i | \sum_{i=1}^n a_{**m**,i} x_i | |


## 補足

<a id="p73"></a> 

### 添え字の訂正
p.73ページの例の中の添字の数字が間違っていました。以下が正しいです。
```
a_{0+1,1}x_1 + a_{0+1,2}x_2 ≦ b_{0+1}
a_{0+2,1}x_1 + a_{0+2,2}x_2 ≦ b_{0+2}
a_{0+3,1}x_1 + a_{0+3,2}x_2 ≦ b_{0+3}
```
<a id="strong_dual"></a> 

### 強双対定理の補足
本書では実行可能な双対問題（実行可能解が存在する双対問題）を解くという話の流れで，
その際に主問題にも最適解が存在すれば良いという書き方をしました．
線形計画問題においては，最適解の存在性を，実行可能解の存在性に置き換えてもよく，強双対定理は以下のようにも記述されます．

**強双対定理**

**主問題と双対問題がどちらも実行可能解を持つならば、どちらにも最適解が存在して、二つの問題の最適値は一致する。**