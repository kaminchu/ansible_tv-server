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

## 実行

```
ansible-playbook -i production site.yml
```
