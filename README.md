# Effective SwiftUI 候補（仮説）

## 効率的な実装
* [プレビュー用に空の SwiftUI プロジェクトを用意する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/9)
* [公式ドキュメントの不足を SwiftOnTap で補う。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/10)
* [新規 View / Modifier を作成する際はスニペットを利用する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/11)
* [body 関数のコンパイルエラーの内容が理解できない場合、小さな関数に移動して試す。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/13)
* 複雑な View 作成時はコードの折りたたみ機能を活用する

## コーディングスタイル
* [サブビューを生成する処理は Computed-property よりメソッドを好む。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/8)
* NavigationView は常に利用する側の View で指定する
* Button の action を関数名で指定しない
* View の構造を把握しやすいような目立つコメントを記述する

## API を理解して使用する
* [本当に必要な場合を除き AnyView を避ける。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/7)
* [UIViewRepresentable のプロトコル要件を正しく理解して使う。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/5)
* [シートを実装する際は Environment の isPresented と dismiss を利用する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/14)
* ObservedObject への DI をonAppearやtaskなどで決して行わない
* ViewModel で非同期通信が必要な場合、MainActorで宣言する

## トレードオフ
* 単純な View に対してのみ Preview を実装する。
* [SFSafeSymbols が本当に必要かよく検討する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/12)
* プラットフォームごとに View を分ける必要があるかよく考える

## テクニック集
* [可読性のための Modifier を導入する。](https://github.com/YusukeHosonuma/Effective-SwiftUI/discussions/6)
* .tagを enum で指定する場合、型付けされた専用のメソッドを用意する
* 必要な場合は型変換用の`Binding`を用意する
* 初期化のために一度だけ実行する処理は`lazy var`で行う

## ネタ枠
* SwiftUI を過信しないこと。
