# 2023年度 エンピリカルソフトウェア工学

## 目的

* 実際のソフトウェア開発でどのようなことが行われているかを実践する．
  * そのために，何らかのアプリケーション（CLIアプリケーション）の開発を行い，ソフトウェア開発の流れを学ぶ．


## 利用する技術

- 開発
  - git/[GitHub](https://github.com/), [GitLab](https://gitlab.com/)
    - Conventional Commits
  - ビルドツール（[Gradle](https://gradle.org/), [Pants](https://www.pantsbuild.org/), [Bazel](https://bazel.build/), [Buck](https://buck.build/), [Please](https://please.build/), [Blade](https://github.com/chen3feng/blade-build)）
  - リリース管理
    - Semantic Versioning
    - DOI（Digital Object Identifier）
  - Web API
    - REST, GraphQL
- テスト
  - UnitTestツール
  - 各種サービス（[codebeat](https://codebeat.co/), [Codacy](https://www.codacy.com/), [Coveralls](https://coveralls.io/) など）
- デプロイ
  - CI/CD
  - [Homebrew](https://brew.sh/index_ja), [Chocolatey](https://community.chocolatey.org/) など
  - [Docker](https://docker.com/), [Podman](https://podman.io/), [Finch](https://github.com/runfinch)
- ドキュメント
  - README, badge
  - [Markdown](https://daringfireball.net/projects/markdown/)
  - 静的サイトジェネレータ（[Jekyll](http://jekyllrb-ja.github.io/), [hugo](https://gohugo.io/), [gatsbyjs](https://www.gatsbyjs.com/)など）
  - 設定記述言語
    - Toml, Yaml, Json, Xml
  

### 利用する言語候補

- Rust
  - https://rust-cli.github.io/book/index.html
- [Go](https://go.dev/)
- [TypeScript](https://www.typescriptlang.org/)（[deno](https://deno.land/)）
- [Kotlin](https://kotlinlang.org/)
- Java（モダンな書き方）
  - [All Loops Are a Code Smell](https://medium.com/swlh/all-loops-are-a-code-smell-6416ac4865d6)
  - [GraalVM](https://www.graalvm.org/) で native code にする．

## 教材候補

* Rust

  * [Command Line Apps in Rust](https://rust-cli.github.io/book/index.html#command-line-apps-in-rust)
  * [Command Line Rust](https://www.oreilly.com/library/view/command-line-rust/9781098109424/)

  * [プログラミング言語Rust](https://doc.rust-jp.rs/book-ja/)

* Kotlin

* TypeScript

* Deno

  * [Effective Deno](https://zenn.dev/uki00a/books/effective-deno)

## 開発候補

### CLI Interface of URL Shortener

短縮URL作成サービス（Bitly，TinyURLなど）と連携して，コマンドラインで短縮URLを取得する．

```sh
surl [GLOBAL_OPTS] <COMMAND>
GLOBAL_OPTS
  -t, --token <TOKEN>   specify the API token.
  -v, --verbose         verbose mode.
  -h, --help            print the help message and exit.
  -V, --version         print the version and exit.
COMMAND
  create   create new shorten url from the given url.
  remove   remove the given shortened urls.
  info     show the information of the given shortened urls.
  list     list the shortened urls and the corresponding urls.
  update   update corresponding url of the given shortened url.
```

### CLI Interface for Weather forecast（天気予報）

CLIで天気予報を取得する．

* [気象庁公式の天気予報API（？）が発見 ～Twitterの開発者界隈に喜びの声が満ちる](https://forest.watch.impress.co.jp/docs/serial/yajiuma/1309318.html)
* [APIキーもログインも不要！完全無料で使える天気予報API「Open-Meteo」を使ってみた！](https://paiza.hatenablog.com/entry/2021/11/04/130000)

```sh
weather [OPTIONS] [LOCATIONs...]
OPTIONS
  -v, --verbose                verbose mode.
  -h, --help                   print this message and exit.
  -V, --version                print the version and exit.
LOCATION
  specify the location in the following ways.
  - Latitude and Longitude,
  - Postal code.
  - The city name.
```



## 進め方

* 第１講（2023-04-11）
  * 言語を決める．
* 第２講（2023-04-18）〜第13講（2023-07-04）
  * 開発
* 第14講（2022-07-11），第15講（2022-07-18）
  * 発表

## 参考資料

* [Command Line Interface Guidelines](https://clig.dev)
  * CLIアプリはどうあるべきかが書かれたサイト．

* [tamada/developing_flows](https://github.com/tamada/developing_flows)
  * ソフトウェア開発でプログラムを書き始める前に行わなければならないことを中心に書いた手引き書．
* [シェルスクリプトを学ぶ人のための「新しいUNIX哲学」 〜 ソフトウェアツールという考え方](https://qiita.com/ko1nksm/items/c55d067b55bbd561df11)
  * これまでに出版されている4つのUNIX哲学を踏まえて，現代のUNIX哲学について解説している．
