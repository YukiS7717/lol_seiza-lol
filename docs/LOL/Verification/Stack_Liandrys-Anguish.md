#ライアンドリーの苦悶のスタックについて
Patch : 12.13
## はじめに
パッチノート12.13が来ましたね。
ライアンドリーの苦悶と悪魔の抱擁に変更がありました。

画像

僕はこれを見たとき思いました。

**スタックってなんだ？**

## 変更前の問題
変更前は複数のチャンピオンがラインドリーの苦悶を所持している場合には、後にスキルを入れたチャンピオンをステータスを参照する仕様でした。
参照値が上書きされてしまうため、サポートとミッドで所持した際に先にミッドが発動したライアンドリーの効果が後にサポートがスキルを発動すると弱いステータスで上書きされてしまう問題がありました。
この問題があるためにライアンドリーの苦悶を同チーム内で複数のチャンピオンが購入することが避けられていました。

## スタック
冒頭でも言いましたが、スタックってなんでしょう。
言葉通りにとらえるのであれば、複数チャンピオンで各々が同時に効果が発動するのでしょうか。それとも先の効果が終了後に後の効果が始まるのでしょうか。
どちらであったとしてもあまりに強すぎます。言葉通りの効果ではないでしょう。

## 検証
### 条件
下記条件で実際に検証してみました。
- チャンピオンA と チャンピオンB がライアンドリーの苦悶を装備する
- チャンピオンC がスキルを受けてデバフアイコンで観測する

### 検証内容
1. チャンピオンA が先にスキルを打つ
2. 2s 後に チャンピオンB がスキルを打つ
3. スキルを受けた チャンピオンC がデバフアイコンを更新しながら観測する

### 結果
結果は下記となりました。

チャンピオンB がスキルを打った時点で チャンピオンB が参照値のライアンドリーの苦悶が有効化される。チャンピオンA が発動していたライアンドリーの苦悶はその時点で終了する。効果時間がリセットされて チャンピオンB のライアンドリーの苦悶が始めからスタートする。

要は後のスキルを打ったチャンピオンの参照値のライアンドリーの苦悶がスタートして、持続中の前の参照値のライアンドリーの苦悶は終わります。

効果時間こそリセットされますが、強い効果を弱い効果で書き換えてしまうので同チームに複数個装備することは推奨できなさそうです。

悪魔の抱擁に関しても同様であると考えられます。
しかし、悪魔の抱擁は参照値がなく相手の最大体力のみを参照とした効果ダメージであるため、複数個装備しても効果延長としては所有しても問題なさそうです。

## おわりに
ライアンドリーの苦悶および悪魔の抱擁のスタックの仕様について検証してみました。
相変わらず効果が読み取りにくい表現でした。
正直スタックするという表現ではなく、効果を新規に発行する等、新しく効果が発生するような表現として欲しかったですね。
スタックだとどうしても重なる意味を想像してしまいます。
