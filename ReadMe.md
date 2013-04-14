# knife-solo版 demo

knife-soloによるDemo環境構築

## 環境構築

```
$ gem install chef
$ gem install knife-solo
```

## 実行手順

```
$ knife solo prepare root@IPアドレス
```
nodesに「IPアドレス.json」ができるので

```
{"run_list":["recipe[demo]"]}
```

と書き込む

```
$ knife cook root@IPアドレス
```

## 参考サイト

[chef-soloとknife-soloで手軽に環境構築をする](http://shrkw.hatenablog.com/entry/configure_with_chef-solo_and_knife-solo)

[knife-soloでLinux環境構築](http://d.hatena.ne.jp/masa21kik/20130210)

[開発メモ#5 : Amazon Linux で knife-solo を使って chef-solo 実行](http://d.hatena.ne.jp/naoya/20130204/1359971408)

