# Visual Studio Codeの設定ファイル

## .vscode

`.vscode`ディレクトリは、Visual Studio Codeの設定ファイルを格納するためのディレクトリです。このディレクトリには、ワークスペースの設定、デバッグ構成、タスク、拡張機能などの設定が含まれています。`.vscode`ディレクトリは、ワークスペースのルートディレクトリに作成されます。このディレクトリは、ワークスペースの設定を共有するために使用されます。


## settings.json

このファイルは、Visual Studio Codeの設定を定義するために使用されます。このファイルには、様々な設定が含まれています。

### editor.codeActionsOnSave

ファイルを保存するときに自動的にインポートを整理するかどうかを制御する設定です。この場合、`source.organizeImports`が`true`に設定されているため、ファイルを保存すると自動的にインポートが整理されます。

### editor.formatOnSave

ファイルを保存するときに自動的にコードをフォーマットするかどうかを制御する設定です。この場合、`true`に設定されているため、ファイルを保存すると自動的にコードがフォーマットされます。

### java.configuration.updateBuildConfiguration

Gradleビルドファイルが変更された場合に自動的に更新するかどうかを制御する設定です。この場合、`automatic`に設定されているため、Gradleビルドファイルが変更された場合に自動的に更新されます。

### java.format.settings.profile

Javaコードをフォーマットするときに使用するプロファイルを設定するための設定です。この場合、`GoogleStyle`に設定されているため、GoogleのJavaコーディングスタイルに従ってコードがフォーマットされます。

### java.format.settings.url

Javaコードをフォーマットするときに使用するフォーマット設定ファイルのURLを設定するための設定です。この場合、GoogleのJavaコーディングスタイルの設定ファイルが指定されています。

## extensions.json

このファイルは、Visual Studio Codeの推奨拡張機能を定義するために使用されます。このファイルには、`recommendations`プロパティが含まれており、このプロパティには、Visual Studio Codeの拡張機能の識別子が含まれています。

### recommendations

`recommendations`プロパティには、Visual Studio Codeの拡張機能の識別子が含まれています。このファイルには、以下の拡張機能が含まれています。

- `editorconfig.editorconfig`: EditorConfigファイルを使用して、コードスタイルを標準化するための拡張機能です。
- `ms-ceintl.vscode-language-pack-ja`: 日本語言語パックを提供する拡張機能です。
- `vscjava.vscode-java-pack`: Java開発に必要な拡張機能をまとめたパックです。

これらの拡張機能は、Visual Studio Codeの開発に役立ちます。

