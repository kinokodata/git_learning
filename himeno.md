# gitの使い方
## gitとは

バージョン管理システム

.から始まるフォルダは隠しフォルダになり、Finderに表示化れない

Subversionというものは以前に使われていた

下位互換ではなく、持っている性質が違い使っているところもある

「差分」という考え方

どのように書き換えたかをgitが管理してくれる

## GitHubからのpull

緑のcodeを押してSSHをコピー

git clone (SSH)で自分のローカルディポジトリになる

`git log` で全てのログが見られる

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

git checkout -b (branch名）

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

## pull request

ちゃんと書けたのでmain branchにか基本で欲しい時に送る

merge requestと同じ

git push→リモートリポジトリに送ろうとする

useから始まるところに「こう書いてね」と出てくるのでマルッとコピー

GitHubに戻り、codeに行くと上に緑のボタンが出てきてそれを押す

create pull  request の緑のボタンを押す（チームリーダーに連絡が行く）

確認してもらって、pull requestのところにメッセージが来る

suggestをもらえることがあるので、それでよければ　commit suggestionを押す（コミットメッセージも送る）

LGTM＝私にとって良いと思います

mergeされたらリモートリポジトリからそのbranchは消える

 <table>
    <tr>
      <th>command</th>
      <th>意味</th>
    </tr>
    <tr>
      <td>mkdir (ディレクトリ名)</td>
      <td>ディレクトリを作る</td>
    </tr>
    <tr>
      <td>cd (ディレクトリ名)</td>
      <td>指定したディレクトリに移動する</td>
    </tr>
     <tr>
      <td>ls -la</td>
      <td>ディレクトリの中身を隠しフォルダを含めてみる</td>
    </tr>
     <tr>
      <td>ls</td>
      <td>ディレクトリの中身を見る</td>
    </tr>
     <tr>
      <td>git clone (SSH)</td>
      <td>ローカルディレクトリにpull</td>
    </tr>
     <tr>
      <td>git log</td>
      <td>ログを見る</td>
    </tr>
     <tr>
      <td>git status</td>
      <td>今の状態を見る</td>
    </tr>
     <tr>
      <td>git commit -m”(コミットメッセージ)”</td>
      <td>commitする</td>
    </tr>
     <tr>
      <td>git push</td>
      <td>GitHubにPushする（useから始まるところをコピーすることが必要かも）</td>
    </tr>
     <tr>
      <td>git branch</td>
      <td>星があるところが今いるところ</td>
    </tr>
     <tr>
      <td>git checkout /b (banch名）</td>
      <td>新しいbranchを作って動く</td>
    </tr>
     <tr>
      <td>git checkout main</td>
      <td>mainに戻る（checkout=branchを切り替える）</td>
    </tr>
  </table>