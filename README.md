# 整体院TAK 経営管理アプリ v2

> 整体院TAKの会計・経営管理アプリ。Firebase Firestore + Vanilla JS + Alpine.js で構築。

## 🎯 役割分担

```
┌─ Coming Soon (1cs.jp) ─────────┐    ┌─ tak-kaikei-v2 ─────────────┐
│ 顧客マスター(1721件)          │    │ 来院記録 / 物販 / 経費        │
│ 予約・カミングメール           │ ←→ │ 広告費 / 現金出納帳           │
└──────────────────────────────┘    │ 月末レポート(Excel自動出力)│
                                       └────────────────────────────┘
```

## 🛠 技術スタック

- HTML + Vanilla JS (Alpine.js 3.x)
- Firebase Firestore (リアルタイム同期、無料枠内)
- Tailwind CSS (CDN)
- GitHub Pages デプロイ

## 🚀 デプロイ

GitHub Pages で自動デプロイ。`main` ブランチへのpushで反映。

URL: https://lag20200401-dotcom.github.io/tak-kaikei-v2/

## 🔐 アクセス

パスコード認証(初期: 1111)

## 📋 開発ロードマップ

- [x] v0.1 - 商品マスターCRUD + Firestore接続
- [ ] v0.2 - 来院記録入力
- [ ] v0.3 - 物販売上入力
- [ ] v0.4 - 経費入力 + 現金出納帳
- [ ] v0.5 - 広告費入力
- [ ] v0.6 - 月末Excel出力(3ファイル)
- [ ] v0.7 - Coming Soon顧客CSV取込
- [ ] v0.8 - 4月分テスト入力
- [ ] v1.0 - 5月途中本番開始
- [ ] v1.x - LINE Messaging API + ビフォアフ自動配信

## ⚠️ Firestoreセキュリティルール

現状「テストモード」(30日後失効)。本番運用前に適切なルール適用が必要。

## 📚 参考ドキュメント

- 設計仕様書: `/integration_設計仕様書_v1.md`
- 引き継ぎドキュメント: `/integration_引き継ぎドキュメント.md`
