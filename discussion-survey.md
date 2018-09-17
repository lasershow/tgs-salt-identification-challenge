## ディスカッション
### カグルイメージセグメンテーションの問題の一般的なトリック
https://www.kaggle.com/c/tgs-salt-identification-challenge/discussion/63984

様々なトリックが記載されている。

### 0.78から0.84+に改善
シンプルなアーキテクチャを利用して、0.84まで改善している。

https://www.kaggle.com/c/tgs-salt-identification-challenge/discussion/65226

### open solution
LB0802 現時点だと最強のsolution
https://www.kaggle.com/c/tgs-salt-identification-challenge/discussion/61949

### データ増強 半教師あり
https://www.kaggle.com/c/tgs-salt-identification-challenge/discussion/63715

### データ増強について
基本的にdata augumentationを行う必要がある
https://www.kaggle.com/c/tgs-salt-identification-challenge/discussion/63974

### シングルモデルでどのくらいか
https://www.kaggle.com/c/tgs-salt-identification-challenge/discussion/64776

#### TTAについて
http://proc-cpuinfo.fixstars.com/2017/06/ai-challenge-contest-01-classification/
(他にも読むべきものがたくさん)

test time augmentation

 モデル平均同様、推論精度を向上させるテクニックです。
これはモデルを複数用意する代わりに、入力画像をData Augmentationで変形させて複数用意しそれぞれの画像に対する確率を平均します。TTAはKaggleのプランクトン画像分類で優勝したチームの記事で知りました。

### 過去と同じコンテスト
https://www.kaggle.com/c/tgs-salt-identification-challenge/discussion/61486
