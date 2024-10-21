[English](README.md) | [日本語(Japanese)](README-ja.md)

# EhiMerPPDB
We release a paraphrase dictionary in Japanese consisting of 380 million phrase pairs. We applied the Bilingual Pivoting method to JParaCrawl, an English-Japanese bilingual corpus, for automatic paraphrase acquisition.

<br>

## Download
We release multiple sizes of paraphrase dictionaries. 
These are filtered paraphrase pairs from the original paraphrase dictionary that have a paraphrase probability below some threshold θ. 
The smaller-scale paraphrase dictionaries have a low recall instead of a high precision.
  |  [S](https://drive.google.com/file/d/1fCRKblzIlxiZWa4bnmf7y1yY_ABRjGpZ/view?usp=sharing) : θ=0.20 |  [M](https://drive.google.com/file/d/1pmThQl4xa3sA9kwWhTamWwJoPrQNL-vv/view?usp=sharing) : θ=0.10 |  [L](https://drive.google.com/file/d/1g0Lt-2qZUF3bXHNWTgOFPyAiRQk_z3N6/view?usp=sharing) : θ=0.05 |  [XL](https://drive.google.com/file/d/11ApNP9xNlLVnSPmT7WD3Q3yRaW2uvloN/view?usp=sharing) : θ=0.01 |  [ALL](https://drive.google.com/file/d/1Lg9mTtH9ZC9sn9P4CF1pJ0zaMrlJfsbm/view?usp=sharing)  |
  | ---- | ---- | ---- | ---- | ---- |
  |  4,964,291  |  8,642,080  |  13,388,634  |  30,379,525  |  386,866,958  |



<br>

## File Format
Our paraphrase dictionaries are distributed as plain text files, with one paraphrase rule per line, as follows:

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
The dictionaries consist of four fields, where ||| is the delimiter. From left to right, original Japanese phrase, paraphrase, paraphrase probability, and English pivot phrases are listed. Note that Japanese phrases are tokenized by MeCab with IPADIC.

<br>

## License
We follow the license of the original JParaCrawl. For more information, please check [here](https://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/).

