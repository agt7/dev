git
=========
複数gitアカウント
```
$ git config --global user.name "メインアカウント"
$ git config --global user.email "メインアカウントメールアドレス"
```

```
cd project_a/
$ git config --local user.name "サブアカウント"
$ git config --local user.email "サブアカウントメールアドレス"
```

認証情報キャッシュ(メモリ)
```
### キャッシュ設定(デフォルト15分)
git config --local credential.helper cache

### 900(15分) => 36000(10時間)
$ vi config
add ↓

[credential]
        helper = cache 30000
```
