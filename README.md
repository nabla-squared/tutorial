# アプリケーション開発手順

Laplacian自動生成基盤を利用したアプリケーション開発を行う際の手順を解説します。

## 事前準備

本手順は **MacOSX** または **Windows10 WSL1 / WSL2** がインストールされた実端末、
もしくは仮想環境(**Docker**コンテナ)上で実施することができます。

本手順を実施する前に、下記の手順のいずれかに従って開発環境を構築してください。

- [開発環境構築手順(MacOSX)](./macosx.md)
- [開発環境構築手順(Windows10 WSL1)](./wsl1.md)
- [開発環境構築手順(Windows10 WSL2)](./wsl2.md)
- [開発環境構築手順(Dockerコンテナ)](./docker.md)

## 作業手順

### [プロジェクトグループの作成](./010_creating_project_group.md)

アプリケーションを構成する各プロジェクトを管理するプロジェクトグループを作成します。

### [アプリケーションドメインモデルの作成](./020_creating_application_domain_model.md)

アプリケーションの問題領域を表現するドメインモデルを作成します。

### [アプリケーションAPIモデルの作成](./030_creating_application_api_model.md)

APIの機能と構成を定義するモデルを作成します。

### [APIサービスの生成と動作確認](./040_generating_and_testing_api_service.md)

アプリケーションAPIモデルから、APIサービスの実装を生成し、ローカルでの動作を確認します。

### [アプリケーションUIモデルの作成](./050_creating_application_ui_model.md)

クライアントアプリケーションのUIを定義するモデルを作成します。

### [Webクライアントアプリケーションの生成と動作確認](./060.md)

アプリケーションUIモデルから、Webクライアントアプリケーションを生成し、ローカルでの動作を確認します。

### [デプロイメントモデルの作成](./070_creating_deployment_model.md)

アプリケーションモデルから生成されたアプリケーションの各種環境へのデプロイを定義するモデルを作成します。

### [クラウド環境へのデプロイ](./080_creating_deployment_model.md)

アプリケーションモデルとデプロイメントモデルからクラウド環境へのデプロイを行うスクリプトを生成し、実際にデプロイを行います。