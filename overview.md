## 概要

- どこに塩山があるかを特定する
- セグメンテーションタスク

## 評価
- IoU

トリックは、IoUしきい値の範囲を掃引し、各点で平均精度値を計算します。閾値は、0.5〜0.95の範囲であり、ステップサイズは0.05：である(0.5, 0.55, 0.6, 0.65, 0.7, 0.75, 0.8, 0.85, 0.9, 0.95)

`IoUについて`
https://www.sigfoss.com/developer_blog/detail?actual_object_id=147

## 提出ファイル

提出ファイルのサイズを縮小するために、我々のメトリックはピクセル値に対してランレングス符号化を使用する。セグメンテーションの索引の完全なリストを提出する代わりに、開始位置と実行長さを含む値のペアを提出します。例えば、「1 3」は、ピクセル1から始まり、合計3ピクセル（1,2,3）を実行することを意味する。

競合形式には、スペースで区切られたペアのリストが必要です。例えば、 '1 3 10 5'は、ピクセル1,2,3,10,11,12,13,14がマスクに含まれることを意味する。ピクセルは、1つのインデックス付きで、上から下に、次に左から右に番号が付けられます.1はピクセル（1,1）、2はピクセル（2,1）などです。

```
id,rle_mask
3e06571ef3,1 1
a51b08d882,1 1
c32590b06f,1 1
etc.
```

## 期限
2018年10月12日  - チーム合併締め切り。これは参加者がチームに参加したりマージしたりする最後の日です。

2018年10月19日  - 最終提出期限。

## データ
- 地震のデータ
- ある特定の地点
- 塩を特定するのは簡単
- 地震画像に加えて、画像化された位置の深さが各画像に提供される

https://www.kaggle.com/c/tgs-salt-identification-challenge/data
