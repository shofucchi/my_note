# Mint セットアップ方法

## 環境

- macOS Big Sur 11.3.1
- Mint 0.16.0

## Mint とは

Swift コマンドラインツールのインストールと実行のパッケージ管理ツール

## Homebrew 経由でインストール

```
$ brew install mint
```

## 使い方

プロジェクトフォルダに`Mintfile`を作成する。

```
cd ProjectFile
touch Mintfile
```

ファイル中身の例  
`{UserName}/{RepositoryName}@{Version} `で記述する。

```
yonaskolb/xcodegen@2.22.0
```

全パッケージのインストール

```
mint bootstrap
```

パッケージの実行例  
`mint run {PackageName} {RunCommand}` で実行する。

```
mint run xcodegen xcodegen generate
```

## 参考

- https://github.com/yonaskolb/Mint#readme
