# README.md: zeam-SWEST-2018-LT

## インストール方法

```
$ gem install slim html2slim redcarpet
$ yarn global add bower yo grunt-cli generator-reveal gulp
$ git clone git@github.com:zeam-vm/zeam-SWEST-2018-LT.git
$ cd zeam-SWEST-2018-LT
$ yarn setup
```

## プレゼンテーション表示方法

```
$ cd zeam-SWEST-2018-LT
$ yarn serve
```

## GitHub Pages への公開

```
$ cd zeam-SWEST-2018-LT
$ yarn deploy
```

[このページを開きます](https://zeam-vm.github.io/zeam-SWEST-2018-LT/)

## スライドの追加

### Markdown のスライドの追加

```
$ cd zeam-SWEST-2018-LT
$ yo reveal:slide "slide-title" --markdown
$ subl slides/slide-title.md
```

next-slide-title には英語のタイトルを入れる(そのままファイル名になる)。残念ながら日本語は通らない。

### HTML のスライドの追加

```
$ cd zeam-SWEST-2018-LT
$ yo reveal:slide "slide-title"
$ subl slides/slide-title.html
```

slide-title には英語のタイトルを入れる(そのままファイル名になる)。残念ながら日本語は通らない。

CSS は css/source/theme.scss を編集する

### Slim のスライドの追加

HTML のスライドの追加をした後，同名の slim ファイルを追加する

```
$ cd zeam-SWEST-2018-LT
$ yo reveal:slide "slide-title"
$ html2slim slides/slide-title.html slides/slide-title.slim
$ subl slides/slide-title.slim
```

slide-title には英語のタイトルを入れる(そのままファイル名になる)。残念ながら日本語は通らない。

CSS は css/source/theme.scss を編集する
