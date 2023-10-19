# 本サイトの使用方法

## 目次
1. * [サンプルサイトのダウンロード方法](#1-サンプルサイトのダウンロード方法)
2. * [ディレクトリ構成](#2-ディレクトリ構成)
3. * [自身で実験サイトを作成する手順](#3-自身で実験サイトを作成する手順)
4. * [外部ライブラリについて](#4-外部ライブラリについて)
5. * [上記の著作権表示および本許諾表示(copyright notice and permission notice)](#5-上記の著作権表示および本許諾表示copyright-notice-and-permission-notice)

## 注意

本マニュアルはGitHub、HTML、CSS、JavaScriptに関して基礎的な知識を持っている方を対象としています。


## 1. サンプルサイトのダウンロード方法

本実験サイトを保存したいディレクトリにて、Windowsであればコマンドプロンプト、Mac OSであればターミナルで以下のコマンドを実行

`git clone https://github.com/hasoseso-Gunnar/PsychologyExperimentSample.git`


## 2. ディレクトリ構成

#### 全体像

root:  
|   .gitignore①  
|   index.html②  
|   README.md③  
|  
+---gas  
|       main.gs④  
|  
+---img⑤  
|       favicon.png  
|  
\---src  
        style.css⑥  

#### ①.gitignore
ローカルレポジトリには保存したいが、GitHubのリモートレポジトリには保存しないファイルを管理するファイル。
後述のgasフォルダーなどの記載を推奨。


#### ②index.html
本実験サイトの核となるファイル。
基本的に、実験サイトの処理に必要なプログラムはここに全て記述する。

後述の「4.外部ライブラリについて」でも述べるように、デフォルトではheadタグ内にて「Vue.js」「Quasar Framework」の2つの外部ライブラリがCDN（Contents Delivery Network）で読み込まれている。


#### ③README.md
本ファイルのこと。後述の「3.自身で実験サイトを作成する手順」 で述べるように、自身で実験サイトを作成する際には削除/gitignoreしてもよい。


#### ④main.gs
実験で得たデータをスプレッドシート等のデータベースに保存する際にGoogle Apps Scriptを使用するのであれば、このファイルの中身を必要に応じて書き換え、
なお、このファイルを含めたgasフォルダーはgitignoreする必要がある。


#### ⑤imgフォルダー
img/配下には実験サイトに用いる画像を置く。


#### ⑥style.css
コンポーネント含め、全てのページにcssを適用したい際には本ファイルを書き換える。


## 3. 自身で実験サイトを作成する手順

加筆予定。


## 4. 外部ライブラリについて

外部ライブラリの詳細な利用マニュアルについては、以下のマニュアルを参照のこと。

#### ①Vue.js(Vue3)
https://ja.vuejs.org/

#### ②Quasar Framework
https://quasar.dev/

#### ③jsPsych(ver 7.3)
https://www.jspsych.org/7.3/

#### ④http-vue-loader
https://github.com/FranckFreiburger/http-vue-loader


## 5. 上記の著作権表示および本許諾表示(copyright notice and permission notice)

#### jsPsych

The MIT License (MIT)

Copyright (c) 2014-2022 Joshua R. de Leeuw

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.