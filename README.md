beamerの使い方とかのメモ
#TeXでプレゼンを作る
##最低必要なもの（テンプレ？）

```tex
\documentclass[dvipdfmx]{beamer}

%表紙の設定
\title{\bfseries タイトル}
\subtitle{サブタイトル}
\author{なまえ}
\institute[]{所属とか}
\date{20xx年x月x日} %日にち

\begin{document}

\begin{frame}
 \titlepage %表紙の表示
\end{frame}

\begin{frame}{スライド１枚目の見出し}
内容とか
\end{frame}

２枚目以降とか

\end{document} %おわり
```

##必要（であろう）パッケージたち
```tex
\usepackage{pxjhyper} %しおりをつける．
\usepackage{graphicx} %画像を使うとき．
\renewcommand{\kanjifamilydefault}{\gtdefault} %日本語フォントをゴシックに．

```

##テーマ（便利なテンプレたち）
いろいろなテンプレが用意されている
```tex
\usetheme{theme} %テーマ
\usecolortheme[named=color]{structure} %テーマの色
```
themeにテーマを書く．例えば，Madridとか．


参考：http://tex.y-misc.org/beamer/theme.html

colorに色を書く．例えば，orangeとか．↑のリンクではすべて青で表示されているがここで色の変更が出来る


参考：http://www2.informatik.uni-freiburg.de/~frank/latex-kurs/latex-kurs-3/farben/Extra-Farben.pdf

##いろいろなコマンド

###ブロック
```tex
\begin{block}{ラベル} 
内容
\end{block}
```
こんな感じのやつが出てくる（theme=Madrid,color=orangeのとき）
[コンパイル後](wiki/beamer.png)

##コンパイル
いつも通りでおｋ．
