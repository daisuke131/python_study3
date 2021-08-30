# Classを活用したレジシステムの構築

Classを使い、小売店などにあるレジシステムの簡易版を作成します。   
Classが理解できると、プログラムをキレイに書けるようになるので是非習得してください！


## task1

マスター登録された商品のメニューを表示してください。  
以下のように各商品の商品コード、商品名、金額を1行ずつ表示しましょう。  

```
001:りんご 100円 
```

また`order.add_item_order("001")`で注文した商品を一覧（一行ずつ）で表示しましょう。
注文した商品の一覧は商品名と金額のみでOKです。

## task2

オーダー`order.add_item_order("001")`の部分をコンソール（ターミナル）から商品コードを入力して登録できるようにしましょう。
繰り返し何度も注文できるようにしましょう。
何も入力しなかった場合は繰り返し処理から抜けましょう。
そのとき内部で注文商品の合計金額を計算しておきましょう。


## task3

task2で注文が終わったあと会計とし、支払い金額を入力できるようにしましょう。
そのときに支払い金額が合計金額を下回った場合は再度、支払い金額を入力させましょう。
支払い金額が合計金額と同額かそれ以上なら、支払い金額とおつりと合計金額を表示しましょう。
これで、注文商品一覧、支払い金額、おつり、合計金額とレシートのようになるはずです。

## task4

ライブラリのpansasを使って商品マスタをitem_master.csvから読み込んで登録できるようにしてください。
各金額で4桁以上はカンマをつけましょう。
支払い金額、おつり、合計金額には円マークをつけましょう。

## task5

商品を注文時さらに個数も注文できるようにしましょう。
レシートの明細にも商品名、金額、個数、小計を表示させましょう。

## task6

レシートを日付時刻をファイル名としたテキストファイルに出力できるようにしてください。
例：2021-01-01-20-01-01.csv
