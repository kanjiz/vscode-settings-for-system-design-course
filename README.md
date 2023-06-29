# Visual Studio Codeの設定ファイル

## .vscode

`.vscode`ディレクトリは、Visual Studio Codeで使用する設定ファイルを保存するためのディレクトリです。このディレクトリには、ワークスペースの設定、デバッグ構成、タスク、拡張機能などの設定が含まれています。`.vscode`ディレクトリは、ワークスペースのルートディレクトリに作成され、複数の開発者が同じ設定を共有するために使用されます。

## settings.json

このファイルには、Visual Studio Codeの様々な設定が含まれています。

### editor.formatOnSave

ファイルを保存するときにコードを自動的に整形するかどうかを設定する項目です。この場合、`true`に設定されているため、ファイルを保存するとコードが自動的に整形されます。つまり、コードを見やすく整えることができます。

```json
{
  "editor.formatOnSave": true
}
```
### java.checkstyle.configuration

Javaコードの品質をチェックするためのCheckstyleの設定ファイルの場所を設定する項目です。Checkstyleは、Javaコードのスタイルや規約に沿っているかどうかをチェックし、問題がある場合には警告やエラーを表示します。`java.checkstyle.configuration`を設定することで、Visual Studio CodeがCheckstyleを使用してJavaコードの品質をチェックするようになります。

```json
{
  "java.checkstyle.configuration": "${workspaceFolder}/config/checkstyle/checkstyle.xml"
}
```

### java.checkstyle.version
Javaコードの品質をチェックするためのツールであるCheckstyleのバージョンを設定する項目です。`java.checkstyle.version`を設定することで、Visual Studio Codeが指定したバージョンのCheckstyleを使用してJavaコードの品質をチェックするようになります。

```json
{
  "java.checkstyle.version": "10.12.1"
}
```

### java.configuration.updateBuildConfiguration

Gradleビルドファイルの変更を自動的に更新するかどうかを設定する項目です。この場合、`automatic`に設定されているため、Gradleビルドファイルが変更された場合に自動的に更新されます。

```json
{
  "java.configuration.updateBuildConfiguration": "automatic"
}
```

### java.format.settings.profile

Javaコードの見た目を整えるために使用するプロファイルを設定する項目です。この場合、`GoogleStyle`に設定されているため、JavaコードをGoogle Java Styleに合わせて整形することができます。つまり、Googleが推奨するJavaコードの書き方に合わせて、コードの見た目を整えることができます。

```json
{
  "java.format.settings.profile": "GoogleStyle"
}
```

### java.format.settings.url

Javaコードの見た目を整えるために使用するフォーマット設定ファイルの場所を設定する項目です。この場合、Google Java Styleの設定ファイルが指定されています。

```json
{
  "java.format.settings.url": "https://raw.githubusercontent.com/google/styleguide/gh-pages/eclipse-java-google-style.xml"
}
```

## extensions.json

このファイルは、以下の4つのおすすめの拡張機能が含まれています。

- `editorconfig.editorconfig`: コードスタイルを標準化するための拡張機能
- `ms-ceintl.vscode-language-pack-ja`: 日本語言語パックを提供する拡張機能
- `shengchen.vscode-checkstyle`: Javaコードの品質をチェックするための拡張機能
- `vscjava.vscode-java-pack`: Java開発に必要な拡張機能をまとめたパック

これらの拡張機能をインストールすることで、Visual Studio Codeでの開発作業がより効率的になり、コードの品質を向上させることができます。
