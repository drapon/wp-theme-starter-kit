# WP Theme Development Kit

WP Theme Development Kitは、WordPressテーマ開発を迅速に開始するための包括的なスターターキットです。現代的な開発ツールとWordPressのベストプラクティスを組み合わせており、開発者が効率的にカスタムテーマを構築できるように設計されています。

## 始め方

このセクションでは、WP Theme Development Kitを使用してプロジェクトを始める方法を説明します。

### 前提条件

- DockerとDocker Composeがインストールされていること。
- WordPressがインストールされていること（オプション）。

### インストール

1. このリポジトリをクローンします。

    ```
    git clone https://github.com/yourusername/wp-theme-development-kit.git
    ```

2. クローンしたディレクトリに移動します。

    ```
    cd wp-theme-development-kit
    ```

### 使用方法

1. 環境変数を設定します。`.env`ファイルに必要な情報を記入してください。

2. ネットワークを作成し、Dockerコンテナを起動します。

    ```
    make up
    ```

   これにより、必要なDockerネットワークが作成され、WordPressとMySQLのコンテナが起動します。

3. 開発が完了したら、コンテナを停止し、削除します。

    ```
    make down
    ```

4. 必要に応じてDockerネットワークも削除できます。

    ```
    make remove-network
    ```

5. すべてをクリーンアップするには、以下のコマンドを使用します。

    ```
    make clean
    ```

### 貢献

このプロジェクトへの貢献に興味がある場合は、プルリクエストを送るか、[Issues](https://github.com/yourusername/wp-theme-development-kit/issues)を通じて提案やフィードバックをお寄せください。

## ライセンス

このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
