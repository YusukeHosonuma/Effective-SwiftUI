# Effective SwiftUI 候補（仮説）

私が SwiftUI で開発する際に **効果的（Effective）** だと感じたプラクティスを記事にしたものです。

元々、Twitter や Zenn のスクラップで書いていたのですが、よりオープンにディスカッションできればと思い、GitHubディスカッションに移行しました（全面的に1からリライトしています）。

どなたもお気軽にリアクション・コメントをいただければと思います。

初めての方は、本ページ下部にある短い [FAQ](#FAQ) にだけ目を通して頂けると幸いです。

## 効率的な実装
* [プレビュー用に空の SwiftUI プロジェクトを用意する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/9)
* [新規 View / Modifier を作成する際はスニペットを利用する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/11)
* [body 関数のコンパイルエラーの内容が理解できない場合、小さな関数に移動して試す。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/13)
* [複雑な View を作成する時は「コードの折りたたみ」機能を活用する](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/2)

## ドキュメント
* [公式ドキュメントの不足を SwiftOnTap で補う。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/10)
* [Apple の公式ドキュメントを参照したい場合は、頭に”Apple SwiftUI”をつけて検索する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/19)

## コーディングスタイル
* [サブビューを生成する処理は Computed-property よりメソッドを好む。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/8)
* [Button における `action` の指定方法について検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/20)
* [View の構造を把握しやすくするために目立つコメントを記述する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/25)

## API を理解して使用する
* [離れた View にデータを渡す際には `@Environment` や `@EnvironmentObject` の利用を検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/28)
* [本当に必要な場合を除き AnyView を避ける。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/7)
* [UIViewRepresentable のプロトコル要件を正しく理解して使う。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/5)
* [シートを実装する際は isPresented と dismiss を利用する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/14)
* [AppStorage で不足な場合は Defaults の利用を検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/23)
* [標準以外の方法でローカライズを処理する際のデメリットを理解する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/29)

## トレードオフ
* [単純な View に対してのみ Preview を実装することを検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/18)
* [SFSafeSymbols が本当に必要かよく検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/12)

## マルチプラットフォーム
* [プラットフォームごとに View を分ける必要があるかよく検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/15)
* [typealias でプラットフォーム間の名前の差異を吸収する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/17)

## テクニック・アイディア集
* [可読性のための Modifier を導入する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/6)
* [.tag() を enum などで指定する場合、型付けされた専用のメソッドを用意する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/16)
* [必要な場合は `Binding<T>` を `Binding<T?>` に変換する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/27)
* [View の更新トリガーを調べるために `_printChanges()` を利用する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/24)

## 未成熟な仮説（私の中で答えが出ていないもの）
* [ViewModel で非同期通信が必要な場合、`@MainActor`で宣言する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/21)
* [NavigationView は常に利用する側の View で指定する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/22)
* [`@ObservedObject` への DI を `onAppear` で決して行わない。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/26)
* [初期化のために一度だけ実行する処理は`lazy var`で行う。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/3)

## FAQ

Q. なんだか文体が偉そう...<br>
A. Effective本を意識して書き始めたら、このような文体になってしまいました...合わない方には申し訳ないです。

Q. 記事リンクを単発でシェアしてもいい？<br>
A. はい、大丈夫です。

Q. 書籍化する予定は？<br>
A. 検討中です。ただ有料の書籍として販売した場合も、ここをクローズするつもりはありません。

Q. あなたは SwiftUI で何を作ったの？<br>
A. <br>
- Multi-platform アプリとしては：
  - [Swift-Evolution-Browser](https://github.com/YusukeHosonuma/Swift-Evolution-Browser)
  - [E2DC](https://github.com/YusukeHosonuma/E2DC)
  - [SwiftUI-LifeGame（古いですが）](https://github.com/YusukeHosonuma/SwiftUI-LifeGame)
- ライブラリとしては：
  - [SwiftUI-Simulator](https://github.com/YusukeHosonuma/SwiftUI-Simulator)
  - [SFReadableSymbols](https://github.com/YusukeHosonuma/SFReadableSymbols)
  - [SwiftUICommon](https://github.com/YusukeHosonuma/SwiftUICommon)
