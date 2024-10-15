[English](README.md) | [日本語(Japanese)](README-ja.md)

# EhiMerPPDB
By applying bilingual pivoting to the English-Japanese corpus JParaCrawl, we have constructed a Japanese paraphrase dictionary with approximately 380 million entries.

<br>

## Download
We set thresholds (0.20, 0.10, 0.05, 0.01) for the paraphrase probability, and set the sizes S, M, L, and XL, respectively.
These thresholds are based on the previous research [PPDB : Japanese](https://ahcweb01.naist.jp/old/resource/jppdb/).

The paraphrase pairs and download URLs included in EhiMerPPDB are as follows:
  |  [S](https://drive.google.com/file/d/1fCRKblzIlxiZWa4bnmf7y1yY_ABRjGpZ/view?usp=sharing)  |  [M](https://drive.google.com/file/d/1pmThQl4xa3sA9kwWhTamWwJoPrQNL-vv/view?usp=sharing)  |  [L](https://drive.google.com/file/d/1g0Lt-2qZUF3bXHNWTgOFPyAiRQk_z3N6/view?usp=sharing)  |  [XL](https://drive.google.com/file/d/11ApNP9xNlLVnSPmT7WD3Q3yRaW2uvloN/view?usp=sharing)  |  [ALL](https://drive.google.com/file/d/1Lg9mTtH9ZC9sn9P4CF1pJ0zaMrlJfsbm/view?usp=sharing)  |
  | ---- | ---- | ---- | ---- | ---- |
  |  4,964,291  |  8,642,080  |  13,388,634  |  30,379,525  |  386,866,958  |


<br>

## About the file
EhiMerPPDB contains the following paraphrase pairs:

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
#### Storage format
Each line contains one paraphrase.
The format is ` paraphrase source phrase ||| paraphrase destination phrase ||| paraphrase probability ||| pivot phrase ` .
The original phrase and the paraphrase destination phrase are tokenized with MeCab and connected with a half-width space.

<br>

## License
Since this dataset is derived from data created based on JParaCrawl, the license follows JParaCrawl.
For more information, please check [here](https://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/).
