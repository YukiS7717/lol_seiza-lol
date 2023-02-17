#ガレン ジャッジメント(E)の回転数について

## はじめに
ガレンのスキル「ジャッジメント」(以後 E)がいつだかのパッチで変更が入りましたね。
E使用時のヒット数がASで変化するようになりました。レベルとアイテムによる上昇ASだけを参照します。回転数も **25 %** のごとに1回ヒット数が増加します。
この仕様により 1-24 % のASは無駄になります。できるだけ25%を少し超えた値を設定できるアイテムを購入できると戦闘能力が上がります。

レベル上昇によるレベルテーブルとアイテムから各レベルにおける装備ASを考察したいと思います。

## ガレン 増加ASステータステーブル
| Level | Attack Speed [%] | 不足分 |
| ----- | ---------------- | ------ |
| 1     | 0.00             | 0.00   |
| 2     | 3.65             | 21.35  |
| 3     | 7.30             | 17.70  |
| 4     | 10.95            | 14.05  |
| 5     | 14.60            | 10.40  |
| 6     | 18.25            | 6.75   |
| 7     | 21.90            | 3.10   |
| 8     | 25.55            | 24.45  |
| 9     | 29.20            | 20.80  |
| 10    | 32.85            | 17.25  |
| 11    | 36.50            | 13.50  |
| 12    | 40.15            | 9.85   |
| 13    | 43.80            | 6.20   |
| 14    | 47.45            | 2.55   |
| 15    | 51.10            | 23.90  |
| 16    | 54.75            | 20.25  |
| 17    | 58.40            | 16.60  |
| 18    | 62.05            | 12.95  |

## ASステータスをもつアイテム
### 素材
| Attack Speed [%] | Item           |
| ---------------- | -------------- |
| 12               | Dagger         |
| 15               | Herthbound Axe |
| 15               | Noonquiver     |
| 15               | Kircheis Shard |
| 18               | Zeal           |
| 25               | Rageknife      |
| 25               | Recurve Bow    |

### ミシック
| Attack Speed [%] | Item               |
| ---------------- | ------------------ |
| 20               | Stridebreaker      |
| 20               | Galeforce          |
| 20               | Immortal Shieldbow |
| 25               | Kraken Slayer      |
| 30               | Trinity Galeforce  |

### レジェンダリー
| Attack Speed [%] | Item                     |
| ---------------- | ------------------------ |
| 15               | Stormrazor               |
| 25               | Blade of The Ruined King |
| 25               | Mortal Reminder          |
| 25               | Phantom Dancer           |
| 35               | Berserker's Greaves      |
| 35               | Rapid Firecannon         |
| 40               | Wit's End                |
| 45               | Guinsoo'sRageblade       |
| 45               | Nashor's Tooth           |

## アイテム選択の方針
- レシオを持たないアイテムはのぞく。
- 18レベル時に再効率となるように選択する。
- 靴をのぞいた2アイテムまでで構成する。

ガレンは回転数以外のスキルレシオはADになるのでAPアイテムは省きます。
また、回転時にはAAを行うことができないため、On Hit Effectのアイテムは極力避けます。
18レベル時の不足増加ASは **12.95 [%]** です。完成品アイテムの増加ASの最小刻み幅が **5 [%]** であるため **25[%]*n + 15[%]** の増加ASを取得できればいいことになります。

## 最終アイテム候補
### 最効率候補 25[%]*n + 15[%]
| 増加回転数 | Item                                                         |
| ---------- | ------------------------------------------------------------ |
| 0          | None                                                         |
| 1          | Stormrazor                                                   |
| 2          | Stormrazor <br> Mortal Reminder                              |
| 2          | Stormrazor <br> Phantom Dancer                               |
| 2          | Wit's End                                                    |
| 3          | Berserker's Greaves <br>  Trinity Force                      |
| 4          | Berserker's Greaves <br>  Trinity Force <br> Mortal Reminder |
| 4          | Berserker's Greaves <br>  Trinity Force <br> Phantom Dancer  |

### 次効率候補 25[%]*n + 20[%]
| 増加回転数 | Item                                    |
| ---------- | --------------------------------------- |
| 0          | None                                    |
| 1          | Stridebreaker                           |
| 1          | Galeforce                               |
| 1          | Immortal Shieldbow                      |
| 2          | Stridebreaker <br> Mortal Reminder      |
| 2          | Stridebreaker <br> Phantom Dancer       |
| 2          | Galeforce <br> Mortal Reminder          |
| 2          | Galeforce <br> Phantom Dancer           |
| 2          | Immortal Shieldbow <br> Mortal Reminder |
| 2          | Immortal Shieldbow <br> Phantom Dancer  |

## 考察結果
上記最終アイテム候補がASを極力無駄なく選択した際のアイテム群になります。

メインの構成アイテムが下記となるのが最も効率がよいと考えられます。
- Stormrazor
- Berserker's Greaves + Trinity Force
- Wit's End

また多少効率は落ちますが、下記をメイン構成としてもよいです。
- Stridebreaker
- Galeforce
- Immortal Shieldbow

このメイン構成に必要に応じて下記アイテムを追加すると効率がよいです。
- Mortal Reminder
- Phantom Dancer  

## ビルドパスについて
ガレンのパワースパイクは下記と考えられます。
このパワースパイクのレベルの際にAS不足を補うアイテムパスを選択するとよいです。

| Level | 不足増加AS |                    |
| ----- | ---------- | ------------------ |
| 6     | 6.75       | ULT習得            |
| 9     | 20.80      | Eのレベルマックス  |
| 10    | 17.25      | パッシブの効果上昇 |
| 11    | 13.50      | ULTレベルアップ    |
| 13    | 6.20       | Qのレベルマックス  |

## おわりに
ガレンの回転数について考察してみました。
アイテムとレベル上昇における値だけを参照するおかげで他のチャンピオンに比べ、無駄が発生しやすいです。
今回の記事でガレンの装備選択の参考になればと思います。
