# Effective SwiftUI 候補（仮説）

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
* NavigationView は常に利用する側の View で指定する
* View の構造を把握しやすいような目立つコメントを記述する

## API を理解して使用する
* [本当に必要な場合を除き AnyView を避ける。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/7)
* [UIViewRepresentable のプロトコル要件を正しく理解して使う。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/5)
* [シートを実装する際は isPresented と dismiss を利用する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/14)
* ObservedObject への DI をonAppearやtaskなどで決して行わない
* ViewModel で非同期通信が必要な場合、MainActorで宣言する

## トレードオフ
* [単純な View に対してのみ Preview を実装することを検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/18)
* [SFSafeSymbols が本当に必要かよく検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/12)

## マルチプラットフォーム
* [プラットフォームごとに View を分ける必要があるかよく検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/15)
* [typealias でプラットフォーム間の名前の差異を吸収する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/17)

## テクニック・アイディア集
* [可読性のための Modifier を導入する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/6)
* [.tag() を enum などで指定する場合、型付けされた専用のメソッドを用意する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/16)
* 必要な場合は型変換用の`Binding`を用意する
* 初期化のために一度だけ実行する処理は`lazy var`で行う

## ネタ枠
* SwiftUI を過信しないこと。
