# Applicationクラスとは

## 概要
- アプリの全ての状態を管理する基底クラス。  
- 通常サブクラスを実装する必要はない。
- サブクラス実装の際は`AndroidManifest.xml`に定義する。

## 知ってること
- Hiltの宣言時にサブクラスとして実装することが多い印象。
- アプリ起動時だけでなく、バックグラウンドで実行するサービスクラスなどアプリに関わる処理が実行される際の最初に呼ばれる。

## 参考
- https://developer.android.com/reference/android/app/Application