# これは何
* Jupyter Notebook 用pdfテンプレート
* ドロップダウンで `Download as` -> `PDF via LaTeX (.pdf)` を選んだときにpdfに日本語が表示されるように修正したテンプレートファイル

# 使い方
`nbconvert`のインストールディレクトリに上書きする

場所を知りたければ
```
pip show nbconvert
```
などでわかる.
* 複数バージョンを共存させている場合はどれがjupyterを動かしているかに注意
* conda系は適当に自分で調べてください

`nbconvert/templates/latex/` に `article.tplx`  を上書きする.

# 注意・補足説明
* 現時点では最低限エラーを出さず, かつ日本語を表示するというだけなので細かいレイアウト調整はしていない.
* コマンドラインでpdfに変換する場合, 自由にテンプレートを選べるが, Notbook上では選べないためとりあえず `article.tplx` に上書きする方法にした.
* `base.tplx` を書き換える方法を掲載しているブログ等あるが, `base.tplx` の内容は他のテンプレートからも読み込まれるので私は**推奨しない**