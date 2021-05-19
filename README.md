# textDiffMaker

- text1 と text2の比較
- text1 の翌日が text2 の想定
- 前日からの差分を出したい。

## 案１
text1を行ごとのリストにして、リストの中身をtext2から検索。見つかれば削除
残ったリストで新text作成

イメージ
text1

```
aaa
bbb
ccc
```

text2
```
aaa
ddd
ccc
```

list1 = (aaa, bbb, ccc)
list2 = (aaa, ddd, ccc)

残るのは、bbbとddd

bbb→ddd
というテキストファイルを生成


## 案２
WinMergeとかで差分の画像を作成
↓
画像をslack送信

- 画像作成を自動化できるのか
- 画像をslack送信ができるのか
