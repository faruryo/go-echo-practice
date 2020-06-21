## 開発環境準備

### 開発ツールインストール

- ホットリロード用として[skaffold](https://skaffold.dev/docs/install/)を使うのでインストールしておく。
- API 動作確認は[Postman](https://www.postman.com/downloads/)を使うのでインストールしておく。
- エディタは[Visual Studio Code](https://code.visualstudio.com/download)を使う
  - 拡張の機能[golang/vscode-go](https://github.com/golang/vscode-go)をインストール

### ホットリロード開発

```bash
skaffold dev --port-forward
```

```
Listing files to watch...
 - faruryo/go-echo-practice
Generating tags...
 - faruryo/go-echo-practice -> faruryo/go-echo-practice:c8e8ce1-dirty
Checking cache...
 - faruryo/go-echo-practice: Not found. Building
Found [docker-desktop] context, using local docker daemon.
Building [faruryo/go-echo-practice]...
[+] Building 3.3s (15/15) FINISHED

・・・・・・・・・・・・・・・・・・・・

Deployments stabilized in 1.588212185s
Port forwarding service/go-echo-practice-api in namespace default, remote port 8080 -> address 127.0.0.1 port 8080
Press Ctrl+C to exit
Watching for changes...
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api]
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api]    ____    __
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api]   / __/___/ /  ___
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api]  / _// __/ _ \/ _ \
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api] /___/\__/_//_/\___/ v4.1.16
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api] High performance, minimalist Go web framework
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api] https://echo.labstack.com
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api] ____________________________________O/_______
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api]                                     O\
[go-echo-practice-api-55c6d8764f-8kj7w go-echo-practice-api] ⇨ http server started on [::]:8080
```

[http://localhost:8080/](http://localhost:8080/)を開く

## 参考

- [【第 4 回】Go 言語（Golang）入門～ REST API 環境構築編～ – 株式会社ライトコード](https://rightcode.co.jp/blog/information-technology/golang-introduction-rest-api)
