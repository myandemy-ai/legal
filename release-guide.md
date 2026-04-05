# Store Release Guide / ストアリリース手順書

最終更新: 20260405

myandemy.ai の App Store / Google Play リリース手順。

---

## 全体フロー

```
1. 事前準備（アカウント・証明書）
2. アプリ設定確認（パッケージ名・アイコン等）
3. ビルド・テスト配布
4. Apple App Store 申請
5. Google Play Store 申請
6. 審査対応
7. リリース後作業
```

---

## 1. 事前準備

### 1-1. 開発者アカウント

| Platform | Account | Cost | Notes |
|---|---|---|---|
| iOS | Apple Developer Program | $99/年 | Myandemy Japan 法人名義 |
| Android | Google Play Console | $25（一回） | Myandemy Japan 法人名義 |

確認事項:
- [ ] Apple Developer: 法人アカウント開設済みか（D-U-N-S番号が必要、取得に2〜4週間）
- [ ] Google Play Console: 本人確認完了済みか（2023年以降義務化）

### 1-2. iOS 証明書・プロファイル

- [ ] App ID 作成（Apple Developer Portal）
- [ ] Distribution Certificate 作成（or 既存を使用）
- [ ] Provisioning Profile（App Store Distribution）作成
- [ ] Push Notification 用の APNs Key

### 1-3. Android 署名キー

- [ ] Upload Key（.jks or .keystore）を生成
- [ ] `key.properties` ファイル作成
- [ ] Google Play App Signing を有効化

---

## 2. アプリ設定確認

### 2-1. パッケージ名・Bundle ID

| Platform | Setting | Value |
|---|---|---|
| iOS | Bundle Identifier | `com.myandemy.ai` |
| Android | applicationId | `com.myandemy.ai` |

- [ ] `ios/Runner.xcodeproj` → Bundle Identifier 確認
- [ ] `android/app/build.gradle` → `applicationId` 確認

### 2-2. アプリ名

- [ ] `android/app/src/main/AndroidManifest.xml` → `android:label`
- [ ] `ios/Runner/Info.plist` → `CFBundleDisplayName`

### 2-3. アプリアイコン

- [ ] 1024x1024px のマスターアイコンを用意
- [ ] `flutter_launcher_icons` で一括生成
- [ ] 各解像度で表示崩れがないか確認

### 2-4. スプラッシュスクリーン

- [ ] `flutter_native_splash` で設定
- [ ] ブランドカラー・ロゴを反映

### 2-5. Firebase / Supabase 設定

- [ ] 本番 Firebase プロジェクト: `google-services.json` (Android) / `GoogleService-Info.plist` (iOS)
- [ ] 本番 Supabase (`eogprqkdmjgyvmriueox`) に接続されていることを確認

### 2-6. その他

- [ ] バージョン番号: `pubspec.yaml` → `version: 1.0.0+1`
- [ ] 最小対応OS: iOS 15.0+ / Android API 24+
- [ ] パーミッション整理（カメラ、通知等）
- [ ] `Info.plist` の Usage Description を日英で記載
- [ ] プライバシーポリシーURL・利用規約URL を設定

---

## 3. ビルド・テスト配布

### 3-1. リリースビルド

```bash
# Android
flutter build appbundle --release

# iOS
flutter build ipa --release
```

- [ ] リリースビルドが正常に完了
- [ ] リリースビルドで実機テスト

### 3-2. 難読化

```bash
# Android
flutter build appbundle --release --obfuscate --split-debug-info=build/debug-info

# iOS
flutter build ipa --release --obfuscate --split-debug-info=build/debug-info
```

### 3-3. テスト配布

- [ ] iOS: TestFlight でベータ配布
- [ ] Android: Google Play 内部テスト or Firebase App Distribution

---

## 4. Apple App Store 申請

### 4-1. App Store Connect 設定

- [ ] 「新規アプリ」作成
- [ ] アプリ名・サブタイトル・カテゴリ入力 → `store-description.md` 参照
- [ ] プライバシーポリシーURL 設定

### 4-2. スクリーンショット

| デバイス | サイズ | 枚数 |
|---|---|---|
| iPhone 6.9" (16 Pro Max) | 1320 x 2868 | 1〜10枚 |
| iPhone 6.7" (15 Plus等) | 1290 x 2796 | 1〜10枚 |
| iPad Pro 13" | 2064 x 2752 | iPad対応の場合 |

- [ ] スクリーンショット作成（日本語・英語・ミャンマー語）
- [ ] アプリ説明文入力 → `store-description.md` 参照
- [ ] キーワード入力
- [ ] What's New 入力

### 4-3. App Privacy

- [ ] App Privacy（データ収集状況）設定 → `../legal/app-store-privacy.md` 参照

### 4-4. アップロード・提出

- [ ] `.ipa` を App Store Connect にアップロード
- [ ] ビルドを選択し、審査に提出
- [ ] 審査チームへのメモ（テストアカウント情報）を記入

### 4-5. よくあるリジェクト理由

- テストアカウント未提供
- プライバシーポリシーのリンク切れ
- データ収集と申告の不一致
- 最小限の機能しかない（Webview ラッパーとみなされる）
- 課金に In-App Purchase を使っていない

---

## 5. Google Play Store 申請

### 5-1. Google Play Console 設定

- [ ] 「アプリを作成」
- [ ] アプリ名・説明文入力 → `store-description.md` 参照

### 5-2. ストア掲載情報

| アセット | サイズ | 必須 |
|---|---|---|
| アプリアイコン | 512 x 512 | Yes |
| フィーチャーグラフィック | 1024 x 500 | Yes |
| スクリーンショット（スマホ） | 最低2枚、16:9 or 9:16 | Yes |
| スクリーンショット（タブレット） | 最低1枚 | タブレット対応時 |

- [ ] スクリーンショット作成
- [ ] フィーチャーグラフィック作成

### 5-3. コンテンツレーティング

- [ ] IARC レーティング質問に回答
- [ ] 対象年齢を設定

### 5-4. データセーフティ

- [ ] データセーフティセクション記入 → `../legal/app-store-privacy.md` を参考に
  - 収集・共有するデータの種類
  - データの暗号化有無
  - データ削除リクエスト対応

### 5-5. アップロード・公開

- [ ] `.aab`（App Bundle）をアップロード
- [ ] テスト配信（内部テスト → クローズドテスト → オープンテスト → 製品版）
- [ ] 製品版リリースを公開

### 5-6. よくあるリジェクト理由

- データセーフティの申告と実際の動作が不一致
- アカウント削除機能がない（2024年以降必須）
- ターゲットAPIレベルが古い
- 広告IDの使用申告漏れ

---

## 6. 審査対応

| | Apple | Google |
|---|---|---|
| 審査期間 | 通常1〜3日 | 通常数時間〜7日 |
| リジェクト時 | Resolution Center で対応 | Policy Status で確認・修正 |
| 再審査 | 修正後に再提出 | 修正後に再提出 |

---

## 7. リリース後作業

- [ ] クラッシュレポート監視（Firebase Crashlytics）
- [ ] アナリティクス確認（DAU, インストール数）
- [ ] ユーザーレビュー対応体制
- [ ] アップデート計画
- [ ] ASO（App Store Optimization）の継続改善

---

## 最終チェックリスト

- [ ] 全画面サイズで正常表示
- [ ] ネットワークエラー時のハンドリング
- [ ] プッシュ通知が正常に届く
- [ ] ログイン・ログアウトが正常動作
- [ ] プライバシーポリシー・利用規約のリンクが有効
- [ ] アカウント削除機能（Apple・Google 両方で必須）
- [ ] 本番 Supabase (`eogprqkdmjgyvmriueox`) に接続
- [ ] デバッグログ・テスト用コードが除去
- [ ] ProGuard/R8 の難読化でクラッシュしない（Android）
- [ ] ATT（App Tracking Transparency）ダイアログ（iOS）
