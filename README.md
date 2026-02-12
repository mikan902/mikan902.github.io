# 管理者ログインシステム - セットアップガイド

## 📋 概要

GitHub Pages用の管理者認証システムです。Supabase Authenticationを使用して、セキュアなログイン機能を提供します。

## 🚀 セットアップ手順

### 1. Supabaseの設定

1. Supabaseダッシュボード (https://app.supabase.com) にアクセス
2. プロジェクト `yjfcbnwfcgcxekintjih` を選択
3. 左サイドバーから「Authentication」→「Users」に移動
4. 「Add user」→「Create new user」をクリック
5. 管理者のメールアドレスとパスワードを入力して作成

### 2. ファイルのアップロード

以下のファイルをGitHubリポジトリにアップロードしてください：

```
mikan902.github.io/
├── index.html           (既存のトップページ)
├── admin-login.html     (ログインページ)
├── admin-dashboard.html (ダッシュボード)
└── README.md            (このファイル)
```

### 3. アクセス方法

- **トップページ**: https://mikan902.github.io/
- **管理者ログイン**: https://mikan902.github.io/admin-login.html
- **ダッシュボード**: https://mikan902.github.io/admin-dashboard.html

## 🔐 セキュリティ機能

✅ **実装済み**
- Supabase認証による安全なログイン
- セッション管理
- 自動ログアウト機能
- 未認証時のリダイレクト保護

## 📱 機能一覧

### ログインページ (admin-login.html)
- メールアドレス・パスワード認証
- エラーメッセージ表示
- レスポンシブデザイン
- ローディング状態表示

### ダッシュボード (admin-dashboard.html)
- ユーザー情報表示
- サイト統計（サンプル）
- クイックアクション
- アクティビティログ
- ログアウト機能

## 🎨 カスタマイズ方法

### 統計情報の更新
`admin-dashboard.html` の以下の部分を編集してください：

```html
<div class="card-value">1,234</div>
```

### カラーテーマの変更
各HTMLファイルの `<style>` セクションで以下の色を変更：

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### 機能の追加
`quick-actions` セクションに新しいボタンを追加：

```html
<button class="action-btn" onclick="yourFunction()">
    🎯 新機能
</button>
```

## 🔧 トラブルシューティング

### ログインできない場合
1. Supabaseでユーザーが正しく作成されているか確認
2. メールアドレスとパスワードが正確か確認
3. ブラウザのコンソールでエラーを確認

### ダッシュボードが表示されない場合
1. ログイン状態を確認
2. ブラウザのキャッシュをクリア
3. プライベートモードで試してみる

### セッションが保持されない場合
1. ブラウザのクッキーが有効か確認
2. Supabaseプロジェクトの設定を確認

## 📞 サポート

問題が発生した場合は、以下を確認してください：
- Supabaseダッシュボードのログ
- ブラウザの開発者ツール（コンソール）
- ネットワークタブでAPIリクエスト

## 🔄 次のステップ

今後追加できる機能：
- [ ] コンテンツ管理機能
- [ ] 画像アップロード
- [ ] アクセス解析の統合
- [ ] 複数管理者のロール管理
- [ ] メール通知機能

---

作成日: 2026年2月12日
バージョン: 1.0.0
