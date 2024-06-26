# GitHub フローに従って開発を進めることができる

GitHub にプッシュをしたことのあるローカルリポジトリ（自分の PC 上のディレクトリ）に移動してください。

## 1. プルリクエストとは

**プルリクエストは何か、何のためにあるかをプログラミング初心者にわかるように説明してください。**  

プルリクエストとは、開発者が変更をおこなったブランチから別のブランチに一連の変更をマージする提案です。  
提案を受けたレビュー・マージ担当者は、コードレビューをおこない問題がなければマージを行います。
問題がある場合は、変更について開発者とコミュニケーションをとり、再度コミットを追加することができます。

## 2. プルリクエストの作成

以下のことを行い、プルリクエストを作成してください。

1. ローカル（自分の PC ）で pullrequest ブランチを新規作成し、切り替えてください
2. 任意のファイルに変更を行ってください
3. 変更をコミットしてください
4. GitHub に pullrequest というブランチ名で変更をプッシュしてください
5. GitHub を開き、pullrequest ブランチから main ブランチへのプルリクエストを作成してください
6. 変更内容を確認し、問題なければ GitHub 上で変更をマージしてください
7. GitHub 上の pullrequest ブランチを削除してください

```shell-session
1.git checkout -b pullrequest

2.vim PULLREQUEST.md

3.git add PULLREQUEST.md
  git commit -v

4.git push origin pullrequest

5.-

6.-

7.-
```

## ３. ローカルへのリポートリポジトリの変更内容の取り込み

ローカルリポジトリのブランチを main ブランチに切り替えてください。

```shell-session
git checkout main
```

次に、リモートリポジトリ（GitHub）の main ブランチの内容をローカルリポジトリの main ブランチに取り込んでください。

```shell-session
git fetch origin main
```

それができたらローカルリポジトリの pullrequest ブランチを削除してください。

```shell-session
git branch -d pullrequest
```

※開発を行う際はここから1に戻り、この1~2のステップを繰り返します

## 4. GitHub フロー

[GitHub フロー](https://docs.github.com/ja/get-started/quickstart/github-flow) の公式リファレンスを一読してください。

その上で、今後の開発は GitHub フローに基づいて行ってください。多くの組織における基本的な開発フローは GitHub フローもしくは GitHub フローをベースにしたものになります。今から GitHub フローに慣れていきましょう。
