# VsCode で dart_style が効かない場合

## 環境

- VsCode: 1.56.0
- DartCode: 3.22.0

## 結論

[こちらの issue](https://github.com/Dart-Code/Dart-Code/issues/1274#issuecomment-587549984)を参考に`setting.json`を修正すれば解決する。

## 原因

どうやら拡張機能として`Prettier`を入れていたのでそことコンフリクトしてたっぽい？  
Dart の場合は上書きするために上記フォーマット設定をする。

## 参考

- [Format document not Working · Issue #1274 · Dart-Code/Dart ...https://github.com › Dart-Code › issues](https://github.com/Dart-Code/Dart-Code/issues/1274)
