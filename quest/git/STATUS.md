# 変更状況を確認できる

Git で管理されているディレクトリに移動してください。任意のファイルに何らかの変更を追加してください。

## 1. 変更状況の確認

現在何のファイルが変更されているかを確認してください。

```shell-session
git status
```

## 2. 変更内容の確認

何が変更されたか、変更内容を確認してください。

```shell-session
git diff
```
```shell-session
git diff --staged
```

## 3. 変更履歴

変更の履歴（ログ）を確認してください。

```shell-session
 git log --oneline
```
