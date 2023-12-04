# アクティビティライフサイクルについて

## 概要
- ライフサイクルとは、システムがアクティビティを起動、再会、中断、破棄している状態のこと。
- Activityにはライフサイクルのコールバック関数が用意されている。
- onCreate
    - アクティビティが作成された際に呼び出される。
    - 必ず実装する。
    - `ViewModel`の関連付けやメンバ変数をインスタンス化したりする。
    - Bundleオブジェクトを受け取れる。
- onStart
    - アクティビティが開始された際に呼び出される。
    - アクティビティがユーザーに表示される。
    - `Lifecycle.Event`の`ON_START`を受け取れる。
- onResume
    - アクティビティが再開された際に呼び出される。
    - アプリフォアグラウンド状態である。
    - `Lifecycle.Event`の`ON_RESUME`を受け取れる。
- onPause
    - アクティビティから離れた際に呼び出される。
    - アプリフォアグラウンド状態ではない。
    - `Lifecycle.Event`の`ON_PAUSE`を受け取れる。
- onStop
    - アクティビティがシステムから停止された際に呼び出される。
    - 別アクティビティが画面全体を占有した場合などに呼び出される。
    - `Lifecycle.Event`の`ON_STOP`を受け取れる。
- onDestroy
    - アクティビティがシステムから破棄された際、構成変更が起きた際に呼び出される。
    - `Lifecycle.Event`の`ON_DESTROY`を受け取れる。

## 知ってること
- 公式はLifecycleObserverでライフサイクルごとの処理を実行するよう強く推奨している。
- onDestroyが実行される構成変更は、`AndroidManifest.xml`に定義することでアクティビティの再生成を抑制することができる。

## 参考
- https://developer.android.com/guide/components/activities/activity-lifecycle?hl=ja
- https://developer.android.com/topic/architecture/recommendations?hl=ja#lifecycle