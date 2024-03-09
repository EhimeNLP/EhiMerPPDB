# EhiMerPPDB
英日対訳コーパス[JParaCrawl](https://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/)に対してBilingual Pivotingを適用することで、約3.8憶件の言い換え辞書を構築しました。

## ダウンロード
```

```

## ファイルについて
EhiMerPPDBには以下のような言い換え対が含まれています。

```
執筆 者 ||| 作家 ||| 0.070106716177562 ||| an author, author ., author whose, author, authors who, authors, authorship, the author, writer, writers
執筆 者 ||| 著者 ||| 0.39808538818661005 ||| author ., author, authors, authorship, the author, the authors, the writer, writer, writers
執筆 者 ||| ライター ||| 0.012387019525242 ||| author, authors, writer, writers
執筆 者 ||| 作者 ||| 0.081727110848016 ||| author, authors who, authors, authorship, the author, the authors, the writer, writer, writers
執筆 者 ||| 筆者 ||| 0.017005844616423002 ||| author, authors, writer, writers
執筆 者 ||| 筆頭 著者 ||| 0.010834235615519999 ||| author, lead author
執筆 者 ||| 著者 は ||| 0.028326534358538203 ||| author, authors, of the authors, the author ,, the author, the authors, the writer, writers
執筆 者 ||| 著者 ら ||| 0.019462660942296997 ||| authors, authorship, the authors
```
#### 格納フォーマット
1行に1つの言い換えが収録されています。  
フォーマットは ` 言い換え元のフレーズ ||| 言い換え先のフレーズ ||| 言い換え確率 ||| ピボット単語 ` です。  
言い換え元のフレーズと言い換え先のフレーズはMeCabでトークナイズされており、半角スペースで接続されています。

#### データサイズ
言い換え確率に対して閾値（0.20，0.10，0.05，0.01）を設定し、それぞれをサイズS，M，L，XLとしています。  
EhiMerPPDBに含まれる言い換え対数は以下の通りです。
  |  S  |  M  |  L  |  XL  |  ALL  |
  | ---- | ---- | ---- | ---- | ---- |
  |  4,964,291  |  8,642,080  |  13,388,634  |  30,379,525  |  386,866,958  |
<br>
  
## ライセンス


## 文献情報
近藤里咲, 梶原智之, 二宮崇. <br>
JParaCrawl からの大規模日本語言い換え辞書の構築. <br>
言語処理学会第30回年次大会, pp.1736-1740, March 2024. \[[PDF](https://www.anlp.jp/proceedings/annual_meeting/2024/pdf_dir/P6-20.pdf)\]
