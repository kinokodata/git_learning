# gitの使い方
## Gitとは

バージョン管理システム

.から始まるフォルダは隠しフォルダになり、Finderに表示化れない

Subversionというものは以前に使われていた

下位互換ではなく、持っている性質が違い使っているところもある

「差分」という考え方

どのように書き換えたかをgitが管理してくれる

## GitHubからのpull

緑のcodeを押してSSHをコピー

git clone (SSH)で自分のローカルディポジトリになる

git logで全てのログが見られる

「q」を押すと終わる

## WebStormでの開き方

開く＞kinokodata＞git_learningを選択して読み込む

## ファイルを書き換える

ターミナルを開いて行う

git status→git add→git commit -m”コミットメッセージ”

origin/main（赤字）→リモートリポジトリ

HEAD→書き換えた最新

git pushでGitHubに書き換えた内容が反映されている

緑→書き加えたこと

赤→消されたところ