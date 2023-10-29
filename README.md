# GitHubリポジトリ検索アプリ

このアプリは、GitHubのリポジトリを検索するためのシンプルなツールです。ユーザーはキーワードを入力し、そのキーワードに基づいてGitHubのリポジトリを検索できます。検索結果は一覧表示され、各リポジトリの詳細情報を表示することができます。

## 機能

- **キーワード入力**: ユーザーは任意のキーワードを入力できます。
- **GitHubリポジトリ検索**: 入力したキーワードに基づいてGitHubのリポジトリを検索します。この機能はGitHub API（search/repositories）を利用しています。
- **検索結果一覧表示**: 検索結果は一覧で表示されます。各アイテムにはリポジトリ名が表示されます。
- **リポジトリ詳細表示**: 検索結果のアイテムをタップすると、該当リポジトリの詳細情報（リポジトリ名、オーナーアイコン、プロジェクト言語、Star数、Watcher数、Fork数、Issue数）が表示されます。
- **エラーハンドリング**: エラーが発生した場合、エラーメッセージが表示されます。「エラーが発生しました。申し訳ございませんが、再度検索してください」というメッセージとともにユーザーに再度検索を促します。

## デザイン

このアプリはマテリアルデザイン3に基づいてデザインされています。シンプルで直感的なUIにより、ユーザーはすばやく簡単に情報を取得できます。

## 注意事項

このアプリはgithub | Dart Packageのようなパッケージを使用せず、API呼び出し処理を自分で実装しています。これにより、アプリの動作がより柔軟になります。

## 使い方

1. アプリを開きます。
2. 検索バーにキーワードを入力します。
3. キーワードに基づいてGitHubのリポジトリが検索され、結果が一覧表示されます。
4. 詳細情報を見たいリポジトリをタップします。該当するリポジトリの詳細情報が表示されます。


## アピールポイント
1. [riverpod](https://riverpod.dev/ja/)を用いてAPIリクエスト時の状態管理を行いました。
   2. 導入時にbranchを切り、安全に実装しました。
2. レスポンスに応じて表示するUIを変更しました。
3. Heroアニメーションを実装しました。
