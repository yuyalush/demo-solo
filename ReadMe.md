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


