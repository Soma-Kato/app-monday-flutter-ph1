# Flutter
## Flutter is 何？
FlutterはGoogleによって開発されたUI ツールキット。（昔はモバイルAppSDKと謳っていた）

```
Flutter is Google’s UI toolkit for building beautiful, natively compiled applications for mobile, web, and desktop from a single codebase.

（Flutter は、単一のコードからmobile、web、desktop向けにネイティブにコンパイルされた美しいアプリケーションを構築するための Google の UI ツールキットです。）
```

---

## 利点
Googleは以下の３つを利点としてあげています。

### Fast Development（開発スピードあがるよ）
- `Hot Reload`を使えばミリ秒単位で、アプリに命を吹き込めるよ。
- `MaterialComponent`などのカスタマイズ可能なウィジェットが最初から入っているから、数分でネイティブアプリの画面を作れるよ。

### Expressive and Flexible UI（表現力と柔軟性に富んだUI）
- だいたい上と同じ

### Native Performance
- Flutter のウィジェットには、スクロール、ナビゲーション、アイコン、フォントなどの重要なプラットフォームの違いがすべて組み込まれている。
<img title='スクリーンショット 2020-07-04 20.00.22.png' src='/attachments/8ad8e73a-acaf-40b5-926c-21df7cfdd4a4' width="1936" data-meta='{"width":1936,"height":444}'>

- Flutter のコードは Dart のネイティブコンパイラを使用してネイティブマシンコードにコンパイルされています。

## もっと詳しく知りたい
- https://flutter.dev/
  
## 導入事例
- StadiaのアプリもFlutter
    - https://medium.com/@ntaoo/flutter-interact-%E3%82%AD%E3%83%BC%E3%83%8E%E3%83%BC%E3%83%88-%E7%99%BA%E8%A1%A8%E5%86%85%E5%AE%B9%E3%81%AE%E3%81%BE%E3%81%A8%E3%82%81-318efa1a291c
- https://qiita.com/usagrammer/items/b05b76f9f67726b7bd4b

# 導入
1. FlutterSDKの取得とPathを通す
    - https://flutter.dev/docs/get-started/install/macos#get-sdk
2. 依存関係を確認
    - `flutter doctor`を実行
        - セットアップを完了するのに必要なToolがあるかを確認してくれます。（XCodeが入っているか、エミュレータの設定が終わっているかなど）
3. iOSエミュレータのセットアップ
    - https://flutter.dev/docs/get-started/install/macos#ios-setup
4. Androidエミュレータのセットアップ
    - https://flutter.dev/docs/get-started/install/macos#android-setup
5. FlutterAppを作成
    - `flutter create my_app`を実行
5. AndroidStudioでBuild


# 
```main.dart
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      theme: ThemeData(
        primarySwatch: Colors.blue,
        visualDensity: VisualDensity.compact,
      ),
      home: //todo,
    );
  }
}
```


# 全体のコードの呼ばれ方

# MaterialAppについて

# Theme周り（どうっすかな）

# Stateless
## 説明
## 簡単な実装（TextOnly）
- build
- hot reload

## 簡単な実装(Button)
- toastを入れてみる
- libStore

# State
## 説明
## 簡単な実装（カウントアップ）
- 公式サンプル
- これをStatelessでやるとどうなるか（試したくない？僕は試した）

# 永続化
## 前置き（いる？）
- Androidやiosは端末のメモリーがなくなるとOSよって立ち上がっていてバックグラウンドに回っているアプリのインスタンスが破棄される。バッテリーなどの問題によって
- sharedPreference lib
- SQL lite lib
## SP
- カウントアップのサンプルをそのまま保存

# 参考
- https://flutter.dev/
-
