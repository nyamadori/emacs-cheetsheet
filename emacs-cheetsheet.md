Emacs チートシート (メモ)
=========================

カーソルの上下移動
--------------

```
行頭 [C-a][C-b] <- カーソル -> [C-f][C-e] 行末
```

```
バッファ先頭
[M-<][Esc <]
  ^
  |
[C-p]
  |
カーソル
  |
[C-n]
  v
[M->][Esc >]
バッファ末尾
```

### 上下

`[C-p]`
: 一行上へ

`[C-n]`
: 一行下へ

`[C-j]`
: 改行

`[M-<]`
: ファイルの先頭へ

`[M->]`
: ファイルの末尾へ

### 左右

`[C-b]`
: 一文字左へ

`[C-f]`
: 一行右へ

`[C-a]`
: 行頭へ

`[C-e]`
: 行末へ


コピー＆ペースト
-------------

### コピー/カット

`[C-SPC]`で選択開始。`[M-w]`でコピー、`[C-w]`でカット。

: 行頭へ

`[C-e]`
: 行末へ


文字の削除
--------

### カーソルの文字削除

```
[C-d]
```

### カーソル位置から行末まで削除

```
[C-k]
```

### バックスペース (カーソルの左側の一文字を削除)

```
[C-h]
```

### カーソル位置の文字を削除

```
[C-d]
```


バッファー操作
-----------

### バッファの切り替え

```
[C-x b]バッファ名
```

### バッファの一覧

```
[C-x C-b]
```

### バッファを画面いっぱいに広げる

現在選択しているバッファをウィンドウいっぱいに広げる。

```
[C-x 1]
```

### バッファを消去する

```
[C-x k]
```

### バッファを上下に2分割

```
[C-x 2]
```

### バッファを左右に2分割

```
[C-x 3]
```


フレーム (ウィンドウ) の操作
-----------------------

### フレーム (ウィンドウ) を作成

```
[C-x 5 2]
```

### フレーム (ウィンドウ) を閉じる

```
[C-x 5 0]
```


アンドゥ・リドゥ
-------------

### アンドゥ

```
[C-x u]
```


検索・置換
---------

### インクリメンタル検索

```
[C-s] 検索文字列
```

### 置換

```
[M-%] 置換対象文字列
```

日本語入力
--------

* 参考
  - http://www.rsch.tuis.ac.jp/~ohmi/literacy/emacs/emacs-jpn.html

### 直接入力と仮名入力をトグル

```
[C-\]
```

### 入力モードを直接入力とひらがな入力でトグルさせる

かな入力モード中に `[qq]` を入力

### 変換中に入力文字列をカタカナに変換

変換中に `[K]` を入力

### 変換中に入力文字列をひらがなに変換

変換中に `[H]` を入力

### 文節

文節縮小
: `[C-i]`

文節拡大
: `[C-o]`

前の文節へ
: `[C-f]`

後ろの文節へ
: `[C-b]`

### 変換

かな漢字変換
: `[SPC]`

変換をリセット
: `[C-c]`

次候補選択
: `[SPC] / [C-n]`

前候補
: `[C-p]`
