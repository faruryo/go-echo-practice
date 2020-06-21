## 開発環境準備

### 開発ツールインストール

- 依存関係管理管理として[dep](https://github.com/golang/dep)を使うのでインストールしておく。
- ホットリロード用として[realize](https://github.com/oxequa/realize)を使うのでインストールしておく。
- API 動作確認は[Postman](https://www.postman.com/downloads/)を使うのでインストールしておく。
- エディタは[Visual Studio Code](https://code.visualstudio.com/download)を使う
  - 拡張の機能[golang/vscode-go](https://github.com/golang/vscode-go)をインストール

### プロジェクト環境設定

依存パッケージインストール

```bash
dep ensure
```

### ホットリロード開発

```bash
realize start
```

```
[02:44:33][GO-ECHO-PRACTICE] : Watching 1 file/s 1 folder/s
[02:44:33][GO-ECHO-PRACTICE] : Install started
[02:44:34][GO-ECHO-PRACTICE] : Install completed in 1.297 s
[02:44:34][GO-ECHO-PRACTICE] : Running..
[02:44:34][GO-ECHO-PRACTICE] :    ____    __
[02:44:34][GO-ECHO-PRACTICE] :   / __/___/ /  ___
[02:44:34][GO-ECHO-PRACTICE] :  / _// __/ _ \/ _ \
[02:44:34][GO-ECHO-PRACTICE] : /___/\__/_//_/\___/ v4.1.16
[02:44:34][GO-ECHO-PRACTICE] : High performance, minimalist Go web framework
[02:44:34][GO-ECHO-PRACTICE] : https://echo.labstack.com
[02:44:34][GO-ECHO-PRACTICE] : ____________________________________O/_______
[02:44:34][GO-ECHO-PRACTICE] :                                     O\
[02:44:34][GO-ECHO-PRACTICE] : ⇨ http server started on [::]:1323
```

[http://localhost:1323/](http://localhost:1323/)を開く

## 参考

- [【第 4 回】Go 言語（Golang）入門～ REST API 環境構築編～ – 株式会社ライトコード](https://rightcode.co.jp/blog/information-technology/golang-introduction-rest-api)
