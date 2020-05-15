# ansible_tv-server

TVサーバーを構築するやつ

# 使い方

## 事前準備

`.ssh/config`に追加する

```
Host tv
  HostName ホスト名
  User ユーザー名
  Port ポート番号
  IdentityFile 鍵
```

pipenv

```
pipenv install
```

## 実行

```
pipenv run ansible-playbook -i production site.yml
```

sudo パスワードが必要なら

```
pipenv run ansible-playbook -i production site.yml --ask-become-pass
```
