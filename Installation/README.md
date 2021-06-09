# 開発環境の準備

このワークショップは Windows でも Mac でも実施することができます。

## 開発ツールのインストール

1. [Visual Studio Code](https://code.visualstudio.com/)
2. Visual Studio Code の [C# 拡張機能](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
3. [.NET Core 3.1 SDK](https://dotnet.microsoft.com/download)

## Tye のインストール

Tye は[グローバルツール](https://docs.microsoft.com/ja-jp/dotnet/core/tools/global-tools)として利用することができます。

以下のコマンドを実行して Tye をインストールします。

```
dotnet tool install -g Microsoft.Tye --version "0.7.0-alpha.21279.2"
```

既に Tye をインストールしている場合は、以下のコマンドでアップデートを行います。

```
dotnet tool update -g Microsoft.Tye --version "0.7.0-alpha.21279.2"
```

以下のコマンドで Tye が正しくインストールできていることを確認します。

```
dotnet tool list -g
```

## 自己証明書の信頼

dotnet SDK を初めてインストールした場合、自己証明書を信頼する必要があるため、以下コマンドを実行します。

```shell
dotnet dev-certs https --trust
```
