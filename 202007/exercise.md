# 20200710 はんなりPython #30 Hanpy Dojo With Kyoto.rb

# 問題１ ループ練習

Hello World![改行]を5回表示させてください。  
print(或いはprintf,cout等)を5回コピーすれば当然可能ですが、
ループ構文(for,while等)を利用して、print等は1回の使用にとどめてみてください。

from http://vipprog.net/wiki/exercise.html#eb2c4338

# 問題2 FizzBuzz

なんか偉い人が考えた問題
ルールは以下の通り

- 1から順番に数を表示する
- その数が3で割り切れるなら"Fizz"、5で割り切れるなら"Buzz"、両方で割り切れるなら"FizzBuzz"と表示する

### 実行例

```
1 2 Fizz 4 Buzz Fizz 7 8 Fizz Buzz 11 Fizz 13 14 FizzBuzz 16 17 Fizz 19 Buzz Fizz 22 23 Fizz Buzz 26 Fizz 28 29 FizzBuzz 31 32 Fizz 34 
```


from http://vipprog.net/wiki/exercise.html#t52e5a48


# 問題3 うるう年測定

入力された整数がグレゴリオ暦（いつも使ってるやつ）でうるう年であるか判定せよ
  
[閏年-wikipedia](https://ja.wikipedia.org/wiki/%E9%96%8F%E5%B9%B4)

> グレゴリオ暦では、次の規則に従って400年間に97回の閏年を設ける。
>
> 1. 西暦年が4で割り切れる年は(原則として)閏年。
> 1. ただし、西暦年が100で割り切れる年は(原則として)平年。
> 1. ただし、西暦年が400で割り切れる年は必ず閏年。

### 出力例

```
1992年はうるう年です
2000年はうるう年です
2001年はうるう年ではありません
```

from http://vipprog.net/wiki/exercise.html#i0d67516

# 問題4 「パトカー」＋「タクシー」＝「パタトクカシーー」

「パトカー」＋「タクシー」の文字を先頭から交互に連結して文字列「パタトクカシーー」を得よ．  
「ハサミ」＋「ペンチ」の文字を先頭から交互に連結して文字列「ハペサンミチ」を得よ．  
「ブラシ」＋「シャモジ」の文字を先頭から交互に連結して文字列「ブシャラモシジ」を得よ．  

from https://nlp100.github.io/ja/ch01.html#02-%E3%83%91%E3%83%88%E3%82%AB%E3%83%BC%E3%82%BF%E3%82%AF%E3%82%B7%E3%83%BC%E3%83%91%E3%82%BF%E3%83%88%E3%82%AF%E3%82%AB%E3%82%B7%E3%83%BC%E3%83%BC


# 問題5 元素記号

**“Hi He Lied Because Boron Could Not Oxidize Fluorine. New Nations Might Also Sign Peace Security Clause. Arthur King Can.”**  

という文を単語に分解し，1, 5, 6, 7, 8, 9, 15, 16, 19番目の単語は先頭の1文字，それ以外の単語は先頭の2文字を取り出し，取り出した文字列から単語の位置（先頭から何番目の単語か）への連想配列（辞書型もしくはマップ型）を作成せよ．


from https://nlp100.github.io/ja/ch01.html#04-%E5%85%83%E7%B4%A0%E8%A8%98%E5%8F%B7


# 問題6 九九

1桁の数値（ 1 ～ 9 に限定）を２つ入力し、その積を表示するプログラムを作成しなさい。  

ただし、九九の計算結果が入った配列を予め作成して利用すること。

from http://kitako.tokyo/lib/JavaExercise.aspx?id=5


---

ここからはAtCoderから出題

---

# 問題7 K-th Common Divisor

### 問題文

正整数 
A
,
B
 が与えられます。

A
 も 
B
 も割り切る正整数のうち、
K
 番目に大きいものを求めてください。

なお、与えられる入力では、
A
 も 
B
 も割り切る正整数のうち 
K
 番目に大きいものが存在することが保証されます。


### 制約


- 入力は全て整数である。
- 1 ≤ A , B ≤ 100 
- A も B も割り切る正整数のうち、K 番目に大きいものが存在する。
- K
≥
1


#### 入力例 1 
```
8 12 2
```
#### 出力例 1 
```
2
```
8
 と 
12
 を割り切る正整数は 
1
,
2
,
4
 です。 この中で 
2
 番目に大きいものは 
2
 です。

#### 入力例 2 

```
100 50 4
```

#### 出力例 2 
```
5
```

from https://atcoder.jp/contests/abc120/tasks/abc120_b


# 問題8 Guidebook

### 問題文
あなたは美味しいレストランを紹介する本を書くことにしました。 あなたは 
N
 個のレストラン、レストラン 
1
、レストラン 
2
、
…
、レストラン 
N
 を紹介しようとしています。レストラン 
i
 は 
S
i
 市にあり、あなたは 
100
 点満点中 
P
i
 点と評価しています。 異なる 
2
 個のレストランに同じ点数がついていることはありません。

この本では、次のような順でレストランを紹介しようとしています。

- 市名が辞書順で早いものから紹介していく。
- 同じ市に複数レストランがある場合は、点数が高いものから紹介していく。
この本で紹介される順にレストランの番号を出力してください。

### 制約
- 1
≤
N
≤
100
- S
 は英小文字のみからなる長さ 
1
 以上 
10
 以下の文字列
- 0
≤
P
i
≤
100
- P
i
 は整数
- P
i
≠
P
j 
(
1
≤
i
<
j
≤
N
)

### 入力
入力は以下の形式で標準入力から与えられる。
```
N
S1 P1
:
SN PN
```

### 出力
N
 行出力せよ。
i
 行目 (
1
≤
i
≤
N
) には、
i
 番目に紹介されるレストランの番号を出力せよ。

#### 入力例 1 
```
6
khabarovsk 20
moscow 10
kazan 50
kazan 35
moscow 60
khabarovsk 40
```

#### 出力例 1 
```
3
4
6
1
5
2
```

3
 種類の市名は辞書順で `kazan` 
<
 `khabarovsk` 
<
 `moscow` です。 それぞれの市について、点数が高いレストランから順に紹介されていきます。よって、レストランは 
3
,
4
,
6
,
1
,
5
,
2
 の順に紹介されていきます。

#### 入力例 2 
```
10
yakutsk 10
yakutsk 20
yakutsk 30
yakutsk 40
yakutsk 50
yakutsk 60
yakutsk 70
yakutsk 80
yakutsk 90
yakutsk 100
```

#### 出力例 2 
```
10
9
8
7
6
5
4
3
2
1
```

from https://atcoder.jp/contests/abc128/tasks/abc128_b



# 問題9 City Savers


### 問題文

N
+
1
 個の街があり、
i
 番目の街は 
A
i
 体のモンスターに襲われています。

N
 人の勇者が居て、
i
 番目の勇者は 
i
 番目または 
i
+
1
 番目の街を襲っているモンスターを合計で 
B
i
 体まで倒すことができます。

N
 人の勇者がうまく協力することで、合計して最大で何体のモンスターを倒せるでしょうか。

### 制約

- 入力は全て整数である。
- 1
≤
N
≤
10^5
- 1
≤
A
i
≤
10^9
- 1
≤
B
i
≤
10^9




### 入力
入力は以下の形式で標準入力から与えられる。
```
N
A1 A2 ... AN+1
B1 B2 ... BN
```
### 出力

合計して倒せるモンスターの数の最大値を出力せよ。



#### 入力例 1 

```
2
3 5 2
4 5
```

#### 出力例 1 
```
9
```
以下のようにモンスターを倒すと、合計 
9
 体のモンスターを倒すことができ、このときが最大です。

- 1
 番目の勇者が 
1
 番目の街を襲っているモンスターを 
2
 体、
2
 番目の街を襲っているモンスターを 
2
 体倒します。
- 2
 番目の勇者が 
2
 番目の街を襲っているモンスターを 
3
 体、
3
 番目の街を襲っているモンスターを 
2
 体倒します。


#### 入力例 2 
```
3
5 6 3 8
5 100 8
```
#### 出力例 2 
```
22
```
#### 入力例 3 
```
2
100 1 1
1 100
```
出力例 3 
```
3
```


from https://atcoder.jp/contests/abc135/tasks/abc135_c


# 問題１0 Crested Ibis vs Monster

### 問題文

トキはモンスターと戦っています。

モンスターの体力は 
H
 です。

トキは 
N
 種類の魔法が使え、
i
 番目の魔法を使うと、モンスターの体力を 
A
i
 減らすことができますが、トキの魔力を 
B
i
 消耗します。

同じ魔法は何度でも使うことができます。魔法以外の方法でモンスターの体力を減らすことはできません。

モンスターの体力を 
0
 以下にすればトキの勝ちです。

トキがモンスターに勝つまでに消耗する魔力の合計の最小値を求めてください。

### 制約
- 1
≤
H
≤
10^4
- 1
≤
N
≤
10^3
- 1
≤
A
i
≤
10^4
- 1
≤
B
i
≤
10^4
- 入力中のすべての値は整数である。


### 入力

入力は以下の形式で標準入力から与えられる。
```
H N
A1 B1
:
AN BN
```

### 出力

トキがモンスターに勝つまでに消耗する魔力の最小値を出力せよ。

#### 入力例 1 
```
9 3
8 3
4 2
2 1
```

#### 出力例 1 

```
4
```

最初に 
1
 番目の魔法を使い、トキの魔力を 
3
 消耗して、モンスターの体力を 
8
 減らします。モンスターの体力は 
1
 になります。

次に 
3
 番目の魔法を使い、トキの魔力を 
1
 消耗して、モンスターの体力を 
2
 減らします。モンスターの体力は 
−
1
 になります。

これにより、トキが消耗した魔力の合計は 
4
 になります。



#### 入力例 2 
```
100 6
1 1
2 3
3 9
4 27
5 81
6 243
```
#### 出力例 2 
```
100
```
1
 番目の魔法を 
100
 回使うのが最適です。



#### 入力例 3 
```
9999 10
540 7550
691 9680
700 9790
510 7150
415 5818
551 7712
587 8227
619 8671
588 8228
176 2461
```

#### 出力例 3 

```
139815
```


from https://atcoder.jp/contests/abc153/tasks/abc153_e
