# 第5章 安全かつ高速なHTTPSサーバの構築

## サンプルコード

**検証のためにオレオレ証明書を使用しています。プロダクション環境では絶対に使用しないでください。**
**各鍵ファイルも必ず作り直してください。**

- [本章で説明した項目を網羅した設定ファイル](nginx.conf)

## 実行方法

443番ポートを使用するため特権権限が必要です。

```
# このディレクトリに移動してください
$ cd nginx-sample/ch3

# フォアグラウンドで起動する場合:
$ sudo nginx -p $(pwd) -c $(pwd)/nginx/3.1-list3.1-nginx.conf -g "daemon off; "

# バックグラウンドで起動する場合:
$ sudo nginx -p $(pwd) -c $(pwd)/nginx/3.1-list3.1-nginx.conf
```