# 2022年度 エンピリカルソフトウェア工学

## 目的

* 実際のソフトウェア開発でどのようなことが行われているかを実践する．
  * そのために，何らかのアプリケーション（CLIアプリケーション）の開発を行い，ソフトウェア開発の流れを学ぶ．


## 利用する技術

- 開発
  - git/[GitHub](https://github.com/), [GitLab](https://gitlab.com/)
  - ビルドツール（[Gradle](https://gradle.org/), [Pants](https://www.pantsbuild.org/), [Bazel](https://bazel.build/), [Buck](https://buck.build/), [Please](https://please.build/), [Blade](https://github.com/chen3feng/blade-build)）
- テスト
  - UnitTestツール
  - 各種サービス（[codebeat](https://codebeat.co/), [Codacy](https://www.codacy.com/), [Coveralls](https://coveralls.io/) など）
- デプロイ
  - CI/CD
  - [Homebrew](https://brew.sh/index_ja), [Chocolatey](https://community.chocolatey.org/) など
  - [Docker](https://docker.com/), [Podman](https://podman.io/)
  - DOI（Digital Object Identifier）
- ドキュメント
  - [Markdown](https://daringfireball.net/projects/markdown/)
  - 静的サイトジェネレータ（[Jekyll](http://jekyllrb-ja.github.io/), [hugo](https://gohugo.io/), [gatsbyjs](https://www.gatsbyjs.com/)など）

### 利用する言語候補

- Rust
  - https://rust-cli.github.io/book/index.html
- [Go](https://go.dev/)（2021年度に利用した）
- [TypeScript](https://www.typescriptlang.org/)（[deno](https://deno.land/)）
- [Kotlin](https://kotlinlang.org/)
- Java（モダンな書き方）（2020年度に利用した）
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

## 進め方

* 第１講（2022-04-12）
  * やること，役割分担を決める．
* 第２講（2022-04-19）〜第５講（2022-05-10）
  * 輪講．
* 第６講（2022-05-17）〜第13講（2022-07-05）
  * 開発
* 第14講（2022-07-12），第15講（2022-07-19）
  * 発表

## 参考資料

* [Command Line Interface Guidelines](https://clig.dev)
  * CLIアプリはどうあるべきかが書かれたサイト．

* [tamada/developing_flows](https://github.com/tamada/developing_flows)
  * ソフトウェア開発でプログラムを書き始める前に行わなければならないことを中心に書いた手引き書．
