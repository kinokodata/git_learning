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

## branch

mainを軸にして、担当する場所ごとなどに枝を生やして作業できる

git checkout /b (banch名）

branch名は機能や名前で

himeno/#1のように書くと良い

書き加えたら　git add (ディレクトリ名)をする

git commit -m”(コミットメッセージ）”でcommitする

branchを切り替えるだけで、作業をなくすことができる

mainはきちんと動く状態、branchでなんやかんや動かしてダメだったら

git checkout mainでbranchを無かったことにできる

自由自在に戻れるし、AとBのbranchで切り替えながら作業ができる

## branchを切り替えながら作業する

git branch→今いる場所の確認

git checkout -b (branch名)→新しいbranchを作る

git add (ディレクトリ名)

git commit -m”(コミットメッセージ）

git log→そのbranchのログを確認

git checkout (いきたいbranch名）→いきたいbranchに移動

commitを細かく分けるのはこういう作業をするため

ピンポイントで作業を直したい時にとても良い