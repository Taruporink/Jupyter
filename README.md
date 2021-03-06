# Jupyter

- [About This Page](#chapter1)
- [Jupyter Notebookの使い方](#chapter2)
- [まとめ](#chapter3)
- [最後に](#chapter4)

## About <a id="chapter1"></a>
[僕のブログ](https://tarupo.xyz/)
で作り紹介したプログラム( 主に白テニ関連 )の多くは，
[このGithub](https://github.com/Taruporink)
に公開してあります．また，
[Jupyter Notebook](http://jupyter.org/)
のファイル形式(.ipynb)で公開してあるものに関しては，利用端末に関わらずブラウザからアクセスして利用することができます．

例えば，
[白猫テニスの個人レートを計算する方法](https://mybinder.org/v2/gh/Taruporink/Jupyter/master?filepath=calcPersonalRate.ipynb)
にアクセスすれば，(やや環境構築に時間がかかりますが)Web上で個人レート計算のプログラムを利用することが可能です．

Jupyterでの公開に適したものは，随時公開して行く予定です．と同時にこの形式で公開したものをWeb上で利用するためのURLをここにまとめておきたいと思います．また，使い方がわからず困る人もいるかもしれないので，簡単に使い方も解説しておこうかなと( より詳しい使い方まで知りたい方は，ググるなりして下さい)．

## Jupyter Notebookの使い方 <a id="chapter1"></a>
まずは最低限の用語を紹介します．

### Cell(セル)
Jupyter Notebookには，Cell(セル)と呼ばれる入力ボックスが存在して，ここにプログラムを書いていくことになります

### Run
画面上部にRunって書いてあるボタンが有ると思います，環境によっては再生ボタン的なマークかも，それを押せばそのセルのプログラムが実行されます．

### メソッドとは
メソッドとは，処理内容を記述しておくもののことで，僕が定義したメソッドを呼び出すことで同じ処理をコンピュータにさせることができます．

メソッドには
**引数**
と呼ばれる値を渡して，その値をもとに計算をします．例えば，ある数xの2乗を計算するプログラムを使いたかったらxを指定しなきゃいけませんよね．そういう感じで必要な情報を引数として渡します．

実行方法は，

``` Python
# これが関数の定義
def hogehoge( x, y=5 ):
    print("サンプルプログラムだよ")

# 実行している↓
hogehoge( 10, y=2 )
```
ってな感じで関数名書いて()で囲んで引数を渡す感じです．

y=5ってなってるのは，引数が渡されなかったらとりあ5で実行するよって感じの意味です．最初はわかりにくいかもですが，触ってみればどうってことはないのでよければなにかしらのを利用してみてください！

### 手順

1. メソッドが記述してあるセル( なんかめっちゃ書いてあるなっていうセル )を選択してRun(実行)する，これでメソッドが定義されます
2. 何も書いてないセルに移動する
3. 適切な引数を渡してメソッドを実行する

## Jupyter Notebookでの利用が可能なリンクまとめ <a id="chapter3"></a>
- [白猫テニス，個人レート特定](https://mybinder.org/v2/gh/Taruporink/Jupyter/master?filepath=calcPersonalRate.ipynb)
- [白猫テニス，レート変動値から層を推定する](https://mybinder.org/v2/gh/Taruporink/Jupyter/master?filepath=層推定ツール.ipynb)
- [Python，論理式から真理値表を生成しプロット](https://mybinder.org/v2/gh/Taruporink/Jupyter/master?filepath=論理式から真理値表への変換.ipynb)

## 最後に <a id="chapter4"></a>
環境ファイルとか僕が用意し忘れると実行できなくなっちゃうので，不具合があれば是非連絡をください．このサイトではコメント機能をつけていないので，
[Twitter](https://twitter.com/tarupo_game)
のほうに連絡を貰えると助かります．
また，利用端末によっては( 特にスマホ，タブレット )環境構築までの時間が長くなるかもしれませんので，その場合は自分でPythonを実行できる環境を用意して実行するのをおすすめします．
