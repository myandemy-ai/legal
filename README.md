# myandemy.ai Store Release

App Store / Google Play リリースに必要な素材の一覧と進捗。

## フォルダ構成

```
store-release/
├── README.md                ← このファイル（素材一覧・チェックリスト）
├── store-description.md     ← ストア掲載テキスト（日/英/ミャンマー語 x App Store/Play Store）
├── release-guide.md         ← リリース手順書（ビルド〜申請〜審査〜リリース後）
├── privacy-policy-ja.md     ← プライバシーポリシー（日本語）
├── privacy-policy-en.md     ← プライバシーポリシー（英語）
├── terms-of-service-ja.md   ← 利用規約（日本語）
├── terms-of-service-en.md   ← 利用規約（英語）
├── tokushoho-ja.md          ← 特定商取引法に基づく表記（日本語）
├── tokushoho-en.md          ← 特定商取引法に基づく表記（英語）
├── app-store-privacy.md     ← App Store Privacy Labels / Google Play Data Safety
└── competitor-research.md   ← 競合調査
```

---

## 素材チェックリスト

### テキスト素材

| 素材 | ファイル | 状態 |
|------|---------|------|
| App Store 説明文（日本語） | `store-description.md` | ✅ |
| App Store 説明文（英語） | `store-description.md` | ✅ |
| App Store 説明文（ミャンマー語） | `store-description.md` | ✅ |
| Play Store 説明文（日本語） | `store-description.md` | ✅ |
| Play Store 説明文（英語） | `store-description.md` | ✅ |
| Play Store 説明文（ミャンマー語） | `store-description.md` | ✅ |
| キーワード（日/英/ミャンマー語） | `store-description.md` | ✅ |
| What's New（日/英/ミャンマー語） | `store-description.md` | ✅ |
| リリース手順書 | `release-guide.md` | ✅ |

### 法的ドキュメント

| 素材 | ファイル | 状態 |
|------|---------|------|
| プライバシーポリシー（日本語） | `privacy-policy-ja.md` | ✅ 20260224 |
| プライバシーポリシー（英語） | `privacy-policy-en.md` | ✅ 20260224 |
| 利用規約（日本語） | `terms-of-service-ja.md` | ✅ 20260224 |
| 利用規約（英語） | `terms-of-service-en.md` | ✅ 20260224 |
| 特定商取引法に基づく表記（日本語） | `tokushoho-ja.md` | ⚠️ TODO 3件 |
| 特定商取引法に基づく表記（英語） | `tokushoho-en.md` | ⚠️ TODO 3件 |
| App Store Privacy Labels | `app-store-privacy.md` | ✅ 20260224 |

### ビジュアル素材

| 素材 | 状態 | 備考 |
|------|------|------|
| アプリアイコン（1024x1024） | ❌ 未作成 | マスター。iOS/Android 各解像度は flutter_launcher_icons で生成 |
| アプリアイコン（512x512） | ❌ 未作成 | Google Play Console 用 |
| スクリーンショット（iPhone 6.9"） | ❌ 未作成 | 1320x2868、各言語、最低1枚 |
| スクリーンショット（iPhone 6.7"） | ❌ 未作成 | 1290x2796、各言語、最低1枚 |
| スクリーンショット（Android） | ❌ 未作成 | 16:9 or 9:16、各言語、最低2枚 |
| フィーチャーグラフィック | ❌ 未作成 | 1024x500、Google Play 必須 |
| スプラッシュスクリーン | ❌ 未作成 | ブランドカラー・ロゴ |

### アカウント・設定

| 項目 | 状態 | 備考 |
|------|------|------|
| Apple Developer Program | ❓ 要確認 | Myandemy Japan 法人名義。D-U-N-S番号が必要 |
| Google Play Console | ❓ 要確認 | Myandemy Japan 法人名義。本人確認必要 |
| iOS Distribution Certificate | ❌ 未作成 | |
| iOS Provisioning Profile | ❌ 未作成 | |
| Android 署名キー (.jks) | ❌ 未作成 | |
| プライバシーポリシー公開URL | ❌ 未定 | Web上に公開が必要 |
| 利用規約公開URL | ❌ 未定 | Web上に公開が必要 |

---

## 未解決事項（TODO）

1. **特商法の未記入項目**（`tokushoho-ja.md`）
   - 電話番号
   - 電話受付時間
   - URL

2. **法的ドキュメントの公開先**
   - プライバシーポリシー・利用規約・特商法をWebで閲覧可能にする必要あり
   - ストア説明文中の `[URL]` を差し替えるため
   - 候補: myandemy.ai ドメインに静的ページ / GitHub Pages / LP サイトに追加

3. **ビジュアル素材の作成**
   - アイコン・スクショ・フィーチャーグラフィックは全て未着手
   - スクリーンショットは実機 or シミュレータで撮影後、キャプション付きデザインに加工

4. **開発者アカウントの開設状況確認**
   - Apple Developer Program（法人）/ Google Play Console の登録状況

5. **ストア説明文のスクショ連動調整**
   - スクリーンショット完成後に説明文を微調整する可能性あり
