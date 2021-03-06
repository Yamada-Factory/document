# Gitコマンド

{% hint style='tip' %}
コマンド操作に不慣れな場合は SourceTree などGUIソフトを使用してください
{% endhint %}


## ブランチの移動
```
$ git switch <移動先ブランチ>
```

## ローカルの更新
リモートの情報をローカルにもってくる
変なことを避けるために masterブランチに移動してやること
```
$ git switch master
$ git pull
```

## ローカルでマージ
ローカルのブランチをマージ
```
$ git merge <merge元ブランチ>
```
リモートのブランチをマージ
```
$ git merge origin/<merge元ブランチ>
```


## ブランチ作成
マージ予定先から切ること！（Git運用参照）
例： `release/v1.0.0` から **feature/add_CNAME#13** というブランチを切るとき
```
$ git switch -c feature/add_CNAME#13 release/v1.0.0

```
### ブランチ作成時のpush
```
$ git push -u origin <作成したブランチ>
```


<br>
<br>
