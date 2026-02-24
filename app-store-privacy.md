# App Store Privacy Details - myandemy.ai

最終更新日: 2026年2月24日 / Last Updated: February 24, 2026

## 技術スタック / Tech Stack

| Component | Service |
|-----------|---------|
| Authentication | Supabase Auth (Email/password, Google SSO) |
| Database | Supabase (PostgreSQL) |
| AI Feature | Google Gemini API |
| Analytics | Google Analytics |
| Push Notifications | Firebase Cloud Messaging (planned) |
| In-App Purchase | App Store / Google Play |
| Advertising | None |

---

## 1. Apple App Privacy Labels

### 1.1 Data Used to Track You / トラッキングに使用されるデータ

Google Analyticsのデバイスベーストラッキングにより、以下のデータがトラッキング目的で使用されます。

| Data Type | Category | Tracked? |
|-----------|----------|----------|
| Device ID | Identifiers | Yes |
| Usage Data (Product Interaction) | Usage Data | Yes |

### 1.2 Data Linked to You / ユーザーに関連付けられたデータ

| Data Type | Category | Collected? | Purpose |
|-----------|----------|------------|---------|
| Email Address | Contact Info | Yes | App Functionality, Developer's Advertising or Marketing |
| Name | Contact Info | Yes | App Functionality |
| User ID | Identifiers | Yes | App Functionality, Analytics |
| Device ID | Identifiers | Yes | Analytics |
| Purchase History | Purchases | Yes | App Functionality |
| Audio Data | User Content | Yes | App Functionality (AI Tutor) |
| Customer Support | User Content | Yes | App Functionality |
| Product Interaction | Usage Data | Yes | Analytics, Product Personalization |

### 1.3 Data Not Linked to You / ユーザーに関連付けられないデータ

| Data Type | Category | Collected? | Purpose |
|-----------|----------|------------|---------|
| Crash Data | Diagnostics | Yes | App Functionality (anonymized) |
| Performance Data | Diagnostics | Yes | App Functionality (anonymized) |
| Product Interaction | Usage Data | Yes | Analytics (aggregated) |

### 1.4 Data Not Collected / 収集しないデータ

以下のデータは収集しません。

- Precise Location / 正確な位置情報
- Coarse Location / おおまかな位置情報
- Physical Address / 住所
- Phone Number / 電話番号
- Contacts / 連絡先
- Photos or Videos / 写真・動画
- Gameplay Content / ゲームコンテンツ
- Browsing History / 閲覧履歴
- Search History / 検索履歴
- Financial Info (payment info, credit card) / 金融情報
- Health & Fitness Data / ヘルスケアデータ
- Sensitive Info / センシティブ情報
- Advertising Data / 広告データ

### 1.5 Apple申請時の選択項目サマリー

**Does your app collect data?**
Yes

**Does your app track users?**
Yes — Device ID and Usage Data are shared with Google Analytics (third-party analytics provider).

**Data types collected (select all that apply):**

| Apple Category | Data Type | Select? |
|---------------|-----------|---------|
| Contact Info | Name | Yes |
| Contact Info | Email Address | Yes |
| Identifiers | User ID | Yes |
| Identifiers | Device ID | Yes |
| Purchases | Purchase History | Yes |
| User Content | Audio Data | Yes |
| User Content | Customer Support | Yes |
| Usage Data | Product Interaction | Yes |
| Diagnostics | Crash Data | Yes |
| Diagnostics | Performance Data | Yes |

**For each data type — Purpose (select all that apply):**

| Data Type | Third-Party Advertising | Developer's Advertising or Marketing | Analytics | Product Personalization | App Functionality |
|-----------|:-:|:-:|:-:|:-:|:-:|
| Name | No | No | No | No | Yes |
| Email Address | No | Yes | No | No | Yes |
| User ID | No | No | Yes | No | Yes |
| Device ID | No | No | Yes | No | No |
| Purchase History | No | No | No | No | Yes |
| Audio Data | No | No | No | No | Yes |
| Customer Support | No | No | No | No | Yes |
| Product Interaction | No | No | Yes | Yes | No |
| Crash Data | No | No | No | No | Yes |
| Performance Data | No | No | No | No | Yes |

**For each data type — Is the data linked to the user's identity?**

| Data Type | Linked to User? |
|-----------|:-:|
| Name | Yes |
| Email Address | Yes |
| User ID | Yes |
| Device ID | Yes |
| Purchase History | Yes |
| Audio Data | Yes |
| Customer Support | Yes |
| Product Interaction | Yes |
| Crash Data | No (anonymized) |
| Performance Data | No (anonymized) |

**For each data type — Is the data used for tracking?**

| Data Type | Used for Tracking? |
|-----------|:-:|
| Device ID | Yes |
| Product Interaction | Yes |
| All other types | No |

---

## 2. Google Play Data Safety Section

### 2.1 Data Shared with Third Parties / 第三者と共有するデータ

| Data Type | Category | Shared With | Purpose |
|-----------|----------|-------------|---------|
| Device ID | Device or other IDs | Google Analytics | Analytics |
| Usage Data (app interactions) | App activity | Google Analytics | Analytics |
| Text input (AI Tutor conversations) | App activity | Google Gemini API | App functionality (core feature) |
| Audio Data (AI Tutor voice input) | Audio | Google Gemini API | App functionality (core feature) |

### 2.2 Data Collected / 収集するデータ

| Data Type | Category | Required? | Purpose |
|-----------|----------|-----------|---------|
| Name | Personal info | Yes | App functionality, account management |
| Email address | Personal info | Yes | App functionality, account management, communications |
| Purchase history | Financial info | Yes | App functionality, subscription management |
| Learning progress | App activity | Yes | App functionality, product personalization |
| In-app actions | App activity | Yes | Analytics, product personalization |
| Crash logs | App info and performance | Yes | App functionality (stability improvement) |
| Diagnostics | App info and performance | Yes | App functionality (performance monitoring) |
| Device ID | Device or other IDs | Yes | Analytics |

### 2.3 Security Practices / セキュリティ対策

| Practice | Status |
|----------|--------|
| Data is encrypted in transit | Yes (HTTPS/TLS) |
| You can request that data be deleted | Yes (account deletion available) |
| Data is transferred using a secure protocol | Yes |
| Built with Google Play's Families policy in mind | No (not a children's app) |
| Independent security review | No [TODO: 将来的にISO 27001取得を検討] |

### 2.4 Google Play申請時の選択項目サマリー

**Does your app collect or share any of the required user data types?**
Yes

**Is all of the user data collected by your app encrypted in transit?**
Yes

**Do you provide a way for users to request that their data is deleted?**
Yes

**Data types (select all that apply):**

| Google Play Category | Data Type | Collected? | Shared? |
|---------------------|-----------|:----------:|:-------:|
| Location | Approximate location | No | No |
| Location | Precise location | No | No |
| Personal info | Name | Yes | No |
| Personal info | Email address | Yes | No |
| Personal info | User IDs | Yes | No |
| Personal info | Address | No | No |
| Personal info | Phone number | No | No |
| Financial info | User payment info | No | No |
| Financial info | Purchase history | Yes | No |
| Health and fitness | — | No | No |
| Messages | — | No | No |
| Photos and videos | — | No | No |
| Audio files | Audio (voice recordings) | Yes | Yes (Gemini API) |
| Files and docs | — | No | No |
| Calendar | — | No | No |
| Contacts | — | No | No |
| App activity | App interactions | Yes | Yes (Analytics) |
| App activity | In-app search history | No | No |
| App activity | Installed apps | No | No |
| App activity | Other user-generated content | Yes | Yes (Gemini API, text input) |
| Web browsing | — | No | No |
| App info and performance | Crash logs | Yes | No |
| App info and performance | Diagnostics | Yes | No |
| App info and performance | Other app performance data | Yes | No |
| Device or other IDs | Device or other IDs | Yes | Yes (Analytics) |

**For each collected data type — Is the data required or optional?**

All collected data types are required for core app functionality.

**For each shared data type — Purpose:**

| Shared Data | Purpose |
|-------------|---------|
| Audio (voice recordings) → Gemini API | Core app functionality (AI Tutor feature) |
| App interactions → Google Analytics | Analytics |
| Other user-generated content → Gemini API | Core app functionality (AI Tutor feature) |
| Device or other IDs → Google Analytics | Analytics |

---

## 3. 補足: 各データ項目の根拠と説明

### 3.1 認証関連 / Authentication

| Data | Source | Explanation |
|------|--------|-------------|
| Email Address | User registration, Google SSO | Supabase Authによる認証に必須。ログイン、パスワードリセット、アカウント通知に使用 |
| Name | User registration, Google SSO | アプリ内の表示名として使用。学習コミュニティ機能での表示 |
| User ID | Auto-generated by Supabase | 内部識別子。学習データ、購入履歴、設定をユーザーに紐付けるために使用 |

### 3.2 AI Tutor関連 / AI Tutor (Gemini API)

| Data | Destination | Explanation |
|------|-------------|-------------|
| Text input | Google Gemini API | AI Tutorとの会話テキスト。レスポンス生成のためにGemini APIに送信される。myandemy.aiはGemini APIのデータ利用ポリシーに準拠 |
| Audio Data | Google Gemini API | 発音練習・会話練習での音声入力。音声認識処理のためにGemini APIに送信される |

Google Gemini API (paid tier) のデータ取り扱い: APIを通じて送信されたデータは、Googleのモデルトレーニングには使用されない（Google Cloud Data Processing Addendum準拠）。

### 3.3 アナリティクス関連 / Analytics (Google Analytics)

| Data | Explanation |
|------|-------------|
| Device ID | Google Analyticsでのユーザー識別に使用。これがApp Storeで「トラッキング」と分類される理由。Google Analyticsは第三者のアナリティクスプロバイダーであり、Device IDをmyandemy.aiのデータと紐付けて分析する |
| Product Interaction | 画面閲覧、ボタンタップ、機能利用頻度などのイベントデータ。UX改善とコンテンツ最適化に使用 |

### 3.4 プッシュ通知 / Push Notifications (Firebase Cloud Messaging)

| Data | Explanation |
|------|-------------|
| FCM Token | Firebase Cloud Messagingが生成するデバイストークン。プッシュ通知の配信に使用。通知機能が実装された時点でプライバシーラベルの更新が必要 [TODO: FCM実装時にラベル更新] |

### 3.5 課金関連 / In-App Purchases

| Data | Explanation |
|------|-------------|
| Purchase History | App Store / Google Play経由のサブスクリプション購入履歴。各プラットフォームが決済処理を行うため、myandemy.aiはクレジットカード番号等の金融情報を直接収集・保持しない |

### 3.6 広告について / Advertising

myandemy.aiは広告を表示しません。Third-Party Advertising目的でのデータ共有はありません。Google Analyticsで使用するDevice IDはAnalytics目的のみです。LingoDeerと同様の広告なしモデルを採用しています。

### 3.7 競合との比較 / Comparison with Competitors

| Feature | myandemy.ai | Duolingo | Busuu | LingoDeer |
|---------|-------------|----------|-------|-----------|
| Tracking data types | 2 (Device ID, Usage) | 8+ | 2 | 1 (Device ID) |
| Third-party advertising | No | Yes | Yes (free tier) | No |
| AI vendor data sharing | Yes (Gemini) | Yes (OpenAI) | Yes (OpenAI, Azure) | No |
| Data collected (categories) | 10 | 19 | 17 | ~8 |
| Ad-free model | Yes | No (free tier has ads) | No (free tier) | Yes |
