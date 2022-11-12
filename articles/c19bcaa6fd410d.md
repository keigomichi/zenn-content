---
title: "マスタリング macOS環境構築 GUIアプリケーション編"
emoji: "🖥️"
type: "idea" # tech: 技術記事 / idea: アイデア
topics: ["macOS", "環境構築"]
published: false
---

この記事は、[Gajeroll Advent Calendar 2022](https://qiita.com/advent-calendar/2022/gajeroll) の 1 日目の記事です。

# 序文

みんなの憧れ MacBook。
快適な macOS ライフを送るには十分なセットアップが欠かせません。
「マスタリング macOS 環境構築」シリーズでは、スピーディーかつ簡単な macOS の環境構築の手順をご紹介します。
この記事では、GUI アプリケーション編と題してこれから Web 開発をはじめる皆さんに、Web 開発者であれば誰もがインストールしているであろうアプリケーションを中心に取り上げていきます。

著者しるす

# Homebrew のインストール

アプリケーションのインストールには Homebrew を使用します。
Homebrew とは macOS や Linux などで使用できるパッケージマネージャーです。
Spotlight で「ターミナル」と検索して、Terminal.app を開きます。ターミナルで以下のコマンドを実行してインストールしてください。

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

https://brew.sh/index_ja

# アプリケーションのインストール

前項でインストールした Homebrew を使用して必要なアプリケーションをインストールしていきます。
Homebrew には、

## iTerm2

iTerm2 は広く使われている macOS 向けのターミナルエミュレーターです。最近では、[Hyper](https://hyper.is/) を使用している方も多い気がします。

```sh
brew install --cask iterm2
```

Homebrew: [https://formulae.brew.sh/cask/iterm2](https://formulae.brew.sh/cask/iterm2)

https://iterm2.com/

## Google Chrome

皆さんご存知の Web ブラウザー。筆者は [Vivaldi](https://vivaldi.com/ja/) も一時期使っていました。Vivaldi は広告ブロック機能や豊富なカスタマイズ性など特徴のあるブラウザーで、Chrome の拡張機能もインストールできます。

```sh
brew install --cask google-chrome
```

Homebrew: [https://formulae.brew.sh/cask/google-chrome](https://formulae.brew.sh/cask/google-chrome)
https://www.google.com/intl/ja_jp/chrome/

## Alfred 5

Alfred は多種多様な作業効率化機能を提供するアプリです。アプリランチャーやファイル検索、電卓などの機能が使えます。課金することでクリップボードやスニペット、ワークフローなどの機能が利用可能になります。
ランチャー系のアプリについては以下の記事で詳しく紹介していますので、ぜひご覧ください。

https://pc.gajeroll.com/

```sh
brew install --cask alfred
```

Homebrew: [https://formulae.brew.sh/cask/alfred](https://formulae.brew.sh/cask/alfred)

https://www.alfredapp.com/

## Slack

2022 年 9 月から、フリープランでは過去 90 日より前の期間のメッセージ履歴とファイルを利用できなくなったことで話題の Slack です。

```sh
brew install --cask slack
```

Homebrew: [https://formulae.brew.sh/cask/slack](https://formulae.brew.sh/cask/slack)

https://slack.com/intl/ja-jp/

## Discord

みんな大好き Discord です。

```sh
brew install --cask discord
```

Homebrew: [https://formulae.brew.sh/cask/discord](https://formulae.brew.sh/cask/discord)

https://discord.com/

## Visual Studio Code

軽量な動作、Git 操作、豊富な拡張機能などスマートな IDE です。
おすすめの VS Code 拡張機能については以下の記事で詳しくご紹介していますので、ぜひご覧ください。

https://pc.gajeroll.com/

[JetBrains](https://www.jetbrains.com/ja-jp/) 製の IDE も定評があります。筆者は [PyCharm](https://www.jetbrains.com/ja-jp/pycharm/) を使ったことがあります。Gopher の方には [GoLand](https://www.jetbrains.com/ja-jp/go/) も人気のようです。

```sh
brew install --cask visual-studio-code
```

Homebrew: [https://formulae.brew.sh/cask/visual-studio-code](https://formulae.brew.sh/cask/visual-studio-code)

https://code.visualstudio.com/

## Rectangle

macOS は、デフォルトでは Windows 風の画面分割操作をすることができません。Rectangle をインストールすれば、キーボードショートカットやマウスのドラッグにより簡単な画面分割を可能にします。

```sh
brew install --cask rectangle
```

Homebrew: [https://formulae.brew.sh/cask/rectangle](https://formulae.brew.sh/cask/rectangle)

https://rectangleapp.com/

## iStat Menus

CPU やメモリの使用率や温度など様々な情報をメニューバーに表示できるシステム監視アプリケーションです。14 日間の無料トライアルの後、$13.19 で利用できます。

```sh
brew install --cask istat-menus
```

Homebrew: [https://formulae.brew.sh/cask/istat-menus](https://formulae.brew.sh/cask/istat-menus)

https://bjango.com/mac/istatmenus/

## Docker

コンテナ技術で仮想環境を構成、共有、実行するアプリケーションです。Docker Desktop では、コンテナーやイメージの一覧を見ることができます。

```sh
brew install --cask docker
```

Homebrew: [https://formulae.brew.sh/cask/docker](https://formulae.brew.sh/cask/docker)

https://www.docker.com/

## Figma

プロトタイプやデザインシステムの作成などいろいろな場面で使えるデザインツールです。Adobe による Figma の買収が話題になりました。

```sh
brew install --cask figma
```

Homebrew: [https://formulae.brew.sh/cask/figmae](https://formulae.brew.sh/cask/figma)

https://www.figma.com/ja/
