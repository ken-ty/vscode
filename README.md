# vscode

VSCodeの設定ファイル置き場。コーディング規約やGUI設定ができる。  
もちろん、プロジェクト毎のコーディング規約を優先します。

## このリポジトリのファイルについて

`tree . ` の結果と各ファイルの要約を示します。

```
.
├── LICENSE        // MIT
├── README.md      // このリポジトリについて
└── settings.json   // vscodeの設定ファイル
```

## settings.json

ctrl + shift + P, preferences: opensettingss (JSON) で表示されるvscodeの設定。
~/.config/Code/User/settingss.json に配置する。
新規端末の初期セットアップ時に一度設定し、後は更新だけ取り込む運用の想定。
ワークスペース毎に置くような使い方はしない。

## editorconfig

プロジェクト毎の設定ファイルの雛形。
ctrl + shift + P, extensions: install extensions, EditorConfig for VS Code をインストールする必要がある。
editorconfigはroot=trueと書かれた.editorconfigが見つかるまでフォルダを遡り、フォルダの上から順番に評価していく。

## 最初に入れる拡張一覧

- Japanese Language Pack for Visual Studio Code

## ナレッジ

〇〇だから××であるべき、的なことをメモする。一旦ここに載せていく。多くなったら整理する。  
このナレッジは、ベストエフォートで設定から自動適用されるべき。

- ファイル末尾には空白行を入れるべき。なぜなら、「行+改行」があって初めて「行」になるから。  
POSIXによると、行とは改行コードで区切られるまでの一連のテキストデータの連続のこと。テキストファイルはいくつかの行の集合体のこと。よって、テキストファイルの末尾には空白行が入るはず。他ファイルも同様に行の集合体と考えるのが良いと思う。  
@see https://bottoms-programming.com/archives/indent-tab-space-and-new-line.html  
@see https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_206
