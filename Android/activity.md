# Activity とは

## 概要
- Androidアプリのエントリポイントを担う重要コンポーネント。
- サブクラス実装の際は`AndroidManifest.xml`に定義する。
- Activityライフサイクルを持つ。
- インテントフィルタを定義することでシステムからのリクエストで起動するアクティビティを定義できる。

## 知ってること
- 以前のAndroid開発では画面=Activityで実装していた。最近は Single Activity + Fragment or Compose で画面構成されることが一般的。  
これは時代によりアプリが複雑化することで遷移方法なども複雑化し、変更がしやすいFragmentなどが画面処理を担うよう移行していった。

## 参考
- https://developer.android.com/guide/components/activities/intro-activities?hl=ja