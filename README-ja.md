# EhiMerPPDB v1.0
英日対訳コーパス[JParaCrawl](https://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/)に対して統計的単語アライメントに基づくBilingual Pivotingを適用することで、約3.8憶件の**日本語言い換え辞書**を構築しました。

<br>

## ダウンロード
言い換え確率に対して閾値（0.20，0.10，0.05，0.01）を設定し、それぞれをサイズS，M，L，XLとしています。  
この閾値の設定は、先行研究である[PPDB : Japanese](https://ahcweb01.naist.jp/old/resource/jppdb/)に倣っています。  
EhiMerPPDB v1.0 に含まれる言い換え対数とダウンロードURLは以下の通りです。

### 日本語版
  |  [S](https://drive.google.com/file/d/1fCRKblzIlxiZWa4bnmf7y1yY_ABRjGpZ/view?usp=sharing)  |  [M](https://drive.google.com/file/d/1pmThQl4xa3sA9kwWhTamWwJoPrQNL-vv/view?usp=sharing)  |  [L](https://drive.google.com/file/d/1g0Lt-2qZUF3bXHNWTgOFPyAiRQk_z3N6/view?usp=sharing)  |  [XL](https://drive.google.com/file/d/11ApNP9xNlLVnSPmT7WD3Q3yRaW2uvloN/view?usp=sharing)  |  [ALL](https://drive.google.com/file/d/1Lg9mTtH9ZC9sn9P4CF1pJ0zaMrlJfsbm/view?usp=sharing)  |
  | ---- | ---- | ---- | ---- | ---- |
  |  4,964,291  |  8,642,080  |  13,388,634  |  30,379,525  |  386,866,958  |

### 英語版
  |  [S](https://drive.google.com/file/d/1-1jJ1DRyAowMcwoiulr5kF9iqbcL7opg/view?usp=sharing)  |  [M](https://drive.google.com/file/d/1OFtEqC7QE-8UwMG0BYSImvdlVOrx4mfx/view?usp=drive_link)  |  [L](https://drive.google.com/file/d/1mtp1V2YHuRNQVv3n0cMPN0x0yhFxQAGh/view?usp=drive_link)  |  [XL](https://drive.google.com/file/d/1MLFdyqys7ngpFXiMA2iSAfYf_tYUk9pH/view?usp=drive_link)  |[ALL](https://drive.google.com/file/d/1DbT834lfUrt0yFd5islV9p4tKZsCsLR-/view?usp=drive_link)|
  | ---- | ---- | ---- | ---- | ---- |
  | 4,427,734 | 7,724,467 | 12,029,243 | 27,606,016 | 250,625,488  |

<br>

## ファイルについて
EhiMerPPDB v1 には以下のような言い換え対が含まれています。

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
各行に1つの言い換えが収録されています。  
フォーマットは ` 言い換え元のフレーズ ||| 言い換え先のフレーズ ||| 言い換え確率 ||| ピボットフレーズ ` です。  
言い換え元のフレーズと言い換え先のフレーズはMeCabでトークナイズされており、半角スペースで接続されています。

<br><br>

# EhiMerPPDB v2.0
英日対訳コーパス[JParaCrawl](https://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/)に対してニューラル単語アライメント（[SimAlign](https://aclanthology.org/2020.findings-emnlp.147/), [PMIAlign](https://aclanthology.org/2023.findings-acl.782/)）に基づくBilingual Pivotingを適用することで、約7,000万件の**日本語言い換え辞書**を構築しました。

<br>

## ダウンロード
EhiMerPPDB v2.0 に含まれる言い換え対数とダウンロードURLは以下の通りです。
### 日本語版
  |  [SimAlignに基づく辞書](https://drive.google.com/file/d/1-zBFYIcckV8Z0pkATmeB0me9J2G7HQfo/view?usp=drive_link)  |  [PMIAlignに基づく辞書](https://drive.google.com/file/d/1z59J0J9YdY_gTpBBdTtzgcYwYykMTSHz/view?usp=drive_link)  |
  | ---- | ---- |
  |  69,345,245  |  71,038,445  |

### 英語版
  |  [SimAlignに基づく辞書](https://drive.google.com/file/d/1lOprmTabe5eSeSbIcYTmr0yJJBQbYre9/view?usp=drive_link)  |  [PMIAlignに基づく辞書](https://drive.google.com/file/d/1Czt0u-mH3_R-FGPk5RRGL4KUZUhq09D8/view?usp=drive_link)  |
  | ---- | ---- |
  |  37,491,481  |  38,157,711 |

#### 格納フォーマット
各行に1つの言い換えが収録されています。  
フォーマットは ` 言い換え元のフレーズ ||| 言い換え先のフレーズ ||| 言い換え確率 ` です。
言い換え元のフレーズと言い換え先のフレーズはMeCabでトークナイズされており、半角スペースで接続されています。


<br>
  
## 文献情報
Risa Kondo, Seiji Sugiyama, Tomoyuki Kajiwara, Takashi Ninomiya. <br>
Paraphrase Acquisition via Bilingual Pivoting Based on Neural Word Alignment. <br>
In Proceedings of the Workshop on Structured Linguistic Data and Evaluation (SLiDE 2026), pp.161-169, Palma, Mallorca, May 2026. \[[PDF](https://www.slide-workshop.org/book.pdf#page=174)\]

近藤 里咲, 梶原 智之, 二宮 崇. <br>
ニューラル単語アライメントに基づく言い換え知識獲得. <br>
言語処理学会第31回年次大会, pp.1488-1492, March 2025. \[[PDF](https://www.anlp.jp/proceedings/annual_meeting/2025/pdf_dir/P4-3.pdf)\]

近藤里咲, 梶原智之, 二宮崇. <br>
JParaCrawl からの大規模日本語言い換え辞書の構築. <br>
言語処理学会第30回年次大会, pp.1736-1740, March 2024. \[[PDF](https://www.anlp.jp/proceedings/annual_meeting/2024/pdf_dir/P6-20.pdf)\]

<br>

## ライセンス
本データセットはJParaCrawlに基づいて作成された派生データであるため、ライセンスはJParaCrawlに従います。  
詳細につきましては[こちら](https://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/)をご確認ください。
