---
layout: post
title:  Slack の使い方
date:   2017-05-15 20:01:14 +0900
tags: slack tutorial
permalink: /
---

とある講義で学生に Slack を使って欲しいので、それの逆引きコレクションです。
順次足していく感じで使っていこうと思う。

# Slack

[Slack](https://slack.com/) はプログラマが好んで使うチャットサービス・ツールである。
[スマホやデスクトップのクライアントアプリ](https://slack.com/downloads)もあるが、ブラウザから利用することもできる。

- チャットは *チーム* と呼ばれる単位で行われる
    - [チームは誰でも作ることができる](https://slack.com/create)
    - [既存のチームに誰でも入れる](https://slack.com/signin)かはチームによる(設定できる)
    - どちらにせよメールアドレスが必要
- チーム内には *チャンネル* と呼ばれる部屋が複数存在する
    - 話題ごとにチャンネルを作成する事が多い
    - ユーザーは任意のチャネルにメッセージを書き込む
- チャンネルには画像などの各種ファイルや *スニペット* と呼ばれるテキストファイルを送信できる
- 各メッセージやファイルには *スレッド* と呼ばれるコメントを残すことができる
- 各メッセージやファイルには *絵文字* でリアクションを追加できる

![ブラウザからの画面]({{site.baseurl}}/assets/images/tutorial-slack/browser.jpg)

# 招待メールが届いたら

![招待メール]({{site.baseurl}}/assets/images/tutorial-slack/invitemail.jpg)

とあるチームから招待されたので、誰から招待されたかが分かるようだったら `Join Now` をクリックする。

![]({{site.baseurl}}/assets/images/tutorial-slack/initsetting1.jpg)

名前(First name)と名字(Last name)と username を入力して `Next` をクリックする。
(username はチャット中に表示されるハンドルネームのようなもので、名前と名字を含め、あとで変更可能である)

![]({{site.baseurl}}/assets/images/tutorial-slack/initsetting1.jpg)

6文字以上のパスワードを設定し、`Next` をクリックする(下のバーが右に行くほど良いパスワード)。

![]({{site.baseurl}}/assets/images/tutorial-slack/initsetting1.jpg)

プライベートポリシーを(よく)読んで、承諾できるなら `I Agree` をクリックする。

![]({{site.baseurl}}/assets/images/tutorial-slack/tutorial.jpg)

チュートリアルの画面が出てくる。
要らなかったら、下の `Skip the tutorial` をクリック。
`Explore Slack` を押すと

![]({{site.baseurl}}/assets/images/tutorial-slack/tutorial1.jpg)

に遷移し、`slackbot` が何かを入力してと言ってるので、何かを入力。

![]({{site.baseurl}}/assets/images/tutorial-slack/tutorial2.jpg)

すると左のサイドバーの説明をしてくれる。
`Next tip` などをクリックしていくとチュートリアルは終了する。

# 画面の構成

![]({{site.baseurl}}/assets/images/tutorial-slack/browser1.jpg)

メッセージにカーソルを合わせると赤枠の様なのが出てくる。

![]({{site.baseurl}}/assets/images/tutorial-slack/message.jpg)

左から

- `add reaction`: 絵文字(スタンプ)をメッセージに付与
- `thread`: スレッドを開始する(Twitterのリプライのようなモノ)
    - スレッド開始後、下のチェックボックスにチェックするとスレッドのメッセージをチャンネルに流してくれる
    - チェックしないとメッセージをクリックしない限り見れない
- `share message`: 引用してメッセージを書き始める(引用ツイートみたいなモノ)
- `…`: その他の操作
    - メッセージの編集や削除ができる

(他にもあるけど、これでだいたいできるはず)

# 特殊文字

- `#randam` のように `#` を付けてメッセージを打つとチャンネルのリンクとなる
- `@hoge` のように `@` を付けてメッセージを打つとユーザーのリンクとなる
- `:no_good:` のように `:` で挟んで打つと絵文字になる(登録されてれば)
- `/` から打つとコマンドの補完がされる
- バッククォート (\`) で挟むとインラインのコードブロックになる
    - 複数行を3つのバッククォートで挟むと複数行のコードブロックになる
- `>` から始めると引用になる
    - `>>>` から始めると改行も含めて以降すべてが引用になる
- `*` で挟むと太字になる
- `_` で挟むと斜体になる
- `~` で挟むと打消し文になる

# ダイレクトメッセージ

Twitter のダイレクトメッセージと同じように、特定の人にメッセージを送ることができる。
しかも、 Slack の場合は複数人(上限は8人)まで同時に送ることができる(8人以上の場合は Private Channel を作りましょう)。

やり方は簡単で左サイドバーの `DIRECT MESSAGES` をクリックする。
すると

![]({{site.baseurl}}/assets/images/tutorial-slack/direct_message.jpg)

のような画面が出てくるので、送信したいユーザーをクリックする。
あとは `Go` を押すと、指定した人たちだけのチャンネルのようなものができるので、そこから普通のチャンネルと同じようにメッセージ送信する。

## スマホアプリでの DM の確認の仕方

左サイドバーを出して(左上のアイコンをクリック)、`Home` を押すと、 `Direct messages` というのが出てくるので、それをクリックする。
