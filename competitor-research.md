# Competitor Legal Document Research / 競合サービス法的ドキュメント調査

Date: 2026-02-12

## Purpose / 目的

myandemy.aiのPrivacy Policy、Terms of Service、App Storeプライバシー情報、特定商取引法表記の作成にあたり、競合する語学学習アプリの法的ドキュメントを調査し、ベストプラクティスを整理する。

---

## 1. Duolingo

**Company**: Duolingo, Inc. (Pittsburgh, PA, USA)
**Privacy Policy**: https://www.duolingo.com/privacy
**Terms of Service**: https://www.duolingo.com/terms
**Common Sense Privacy Rating**: 58% (Warning)

### 1.1 Privacy Policy

#### Data Collected
- **Account Data**: Name, email, age, phone number, password
- **Social Login Data**: Google/Facebook/Appleアカウントからのメール、場合によっては連絡先
- **Learning Data**: 学習言語、完了スキル・レッスン、単語強度、個人辞書
- **Usage Data**: アプリ利用時間・頻度、アプリ内購入
- **Device Data**: デバイスタイプ、OS、アプリバージョン、IPアドレス
- **Voice Data**: 発音練習用の音声（Google/Apple/AWSの第三者プロバイダーに送信）
- **Exam Data (DET)**: 政府発行の身分証明書写真、顔写真、ウェブカメラ・マイク録画
- **合計19データポイント**を収集（業界平均より多い）

#### AI Data Handling
- Duolingo MaxはOpenAIのGPT-4を使用（AI Tutor機能）
- AI機能利用時、ユーザー情報はOpenAI等のAIベンダーと共有される
- **OpenAIがテキスト・音声レスポンスのコピーを自社目的で保持する可能性あり**（Privacy Policyに明記）
- 音声データはサーバー到着時に匿名化

#### Children's Privacy (COPPA)
- 13歳未満の子供からの個人情報収集には保護者の同意が必要
- 子供のプロフィールは非公開・検索不可
- ソーシャル機能を制限
- 保護者のメールアドレスでのみアカウント作成可能
- 名前や年齢等の個人識別情報は提供不可

#### International Data Transfer
- Duolingo, Inc.がGDPR上のデータコントローラー
- 国際転送の契約上の保護については明確な記載なし

#### User Rights (GDPR/CCPA)
- アカウント設定からデータのアクセス・修正・削除が可能
- メール通知でもデータ管理リクエスト可能
- CCPA: カリフォルニア州の消費者プライバシー権に準拠

#### Data Retention
- アカウント終了時にデータ削除
- 匿名化された試験データは研究目的で無期限保持の可能性
- 具体的な削除タイムラインは不明確

#### Third-Party Sharing
- 広告ネットワーク、マーケティング分析、ウェブサイト分析企業とデータ共有
- Google、Facebook、Oath、Unityなどのパートナー
- 個人データの第三者への「販売」はしないと主張
- Do Not Track信号には応答しない

### 1.2 Terms of Service

ToS;DR Grade: **C**

#### Subscription & Auto-Renewal
- プロフィール設定から自動更新のオフが可能
- 請求サイクル終了の24時間前までにキャンセル必要
- 返金ポリシーなし

#### User-Generated Content (UGC)
- ユーザーはUGCの所有権を保持（著作者人格権の放棄不要）
- プロフィールはデフォルトで公開、UGCも公開される可能性
- コミュニティガイドライン違反のスキャン・削除権限あり
- 第三者コンテンツモデレーションサービスとの共有可能性

#### AI Disclaimers
- AI機能利用時のデータ共有についてPrivacy Policyで言及あるが、ToSでのAI固有の免責事項は限定的

#### Key Positive Points
- ユーザーがUGCの所有権を保持
- 規約変更の1週間前通知
- マーケティングメールの簡易オプトアウト

### 1.3 Apple App Privacy Labels

#### Data Used to Track You
Purchases, Location, Contact Info, User Content, Identifiers, Usage Data, Diagnostics, Other Data

#### Data Linked to You
- **Third-Party Advertising**: Purchase History, Coarse Location, User ID, Device ID, Product Interaction, Advertising Data
- **Analytics**: Purchases, Location, Contact Info, User Content, Search History, Identifiers, Usage Data, Diagnostics
- **App Functionality**: Purchases, Financial Info, Location, Contact Info, Contacts, User Content, Identifiers, Diagnostics

**Note**: 収集データの2/3（19中13ポイント）をトラッキング目的で使用（業界平均の4倍）

---

## 2. Busuu

**Company**: Busuu Limited (subsidiary of Chegg, Inc.)
**Privacy Policy**: https://www.busuu.com/en/privacy (+ Chegg Privacy Policyが補完)
**Terms of Service**: https://www.busuu.com/en/terms
**Certification**: ISO/IEC 27001:2022 Information Security and Privacy Standard
**PrivacySpy Rating**: 5.1/10

### 2.1 Privacy Policy

#### Data Collected
- **Registration Data**: ユーザー名、メール、学習言語、プロフィール写真
- **Automatically Collected**: サービスメタデータ、ログデータ、デバイス情報、IPアドレス、サードパーティデータ、Cookie情報
- **Learning Data**: コンテンツ消費、回答、コース進捗、熟達度、レッスン消費、流暢度スコア、証明書
- **Voice/Audio Data**: Speaking Practice機能での音声録音
- **合計17データポイント**を収集
- **除外**: 健康データ、生体認証情報、犯罪記録は収集しない（明示的に記載）

#### AI Data Handling
- AI Conversation Practice: OpenAI等のサービスプロバイダーが一部機能を提供
- 音声は録音・保持され、サービス提供と改善に使用
- **音声情報は機械学習モデルのトレーニングに使用**（専門の人間レビュアーの支援付き）
- 音声はユーザーの固有識別には使用しない
- Azure AI Speech servicesを使用

#### Children's Privacy
- 明確な記載なし（Chegg Privacy Policyに委ねている可能性）

#### International Data Transfer
- データコントローラー: Chegg, Inc.
- BusuuのSupplemental Privacy PolicyがChegg Privacy Policyを補完

#### User Rights (GDPR/CCPA)
- privacy@busuu.com へのメールでデータ削除リクエスト可能
- 法的要件により一部の金融情報は保持
- research@busuu.com で研究参加の取り消し可能

#### Data Retention
- 一部のUser Content（コメント、投稿、メッセージ）はプロフィール削除後も残存する可能性
- 最終更新: 2019年8月（比較的古い）

#### Third-Party Sharing
- 広告主: Facebook, Google, Braze, Snapchat（ターゲティングマーケティング用）
- **Premium会員は広告表示なし、広告目的のデータ共有なし**
- 法執行機関への開示: 召喚状、裁判所命令、法的手続き対応時
- サードパーティサービスプロバイダーには指定目的以外のデータ利用を制限

### 2.2 Terms of Service

#### Subscription & Auto-Renewal
- App Store購入の場合、App Storeの規約にも準拠
- キャンセルは各プラットフォーム（Web/App Store）で直接行う
- 更新料金を避けるには24時間前までにキャンセル

#### Cancellation & Refund
- **14日間返金保証**: 初回Premium加入時のみ適用
- 自動更新・その他の課金サイクルには返金不可
- キャンセル後も支払い済み期間の終了まではPremiumアクセス継続

#### User Content
- プロフィール削除後、一部のUser Content（コメント等）は残存可能性

### 2.3 Apple App Privacy Labels

#### Data Used to Track You
Identifiers, Usage Data

#### Data Linked to You
- Purchase History, Coarse Location, Email, Name, Phone Number
- Photos/Videos, Audio Data, Support Interactions
- User ID, Device ID, Product Interaction, Advertising Data
- Crash Data, Performance Data

**Purposes**: Third-Party Advertising, Developer's Advertising/Marketing, Analytics, Product Personalization, App Functionality

---

## 3. LingoDeer

**Company**: LingoDeer (HQ location not prominently disclosed)
**Privacy Policy**: https://lingodeer.com/privacypolicy-html
**Terms of Service**: https://www.lingodeer.com/terms-conditions-html

### 3.1 Privacy Policy

#### Data Collected
- アカウント情報（メール、名前等）
- デバイス情報（ID、OS等）
- 学習進捗データ
- 音声データ（発音分析のため第三者サービスプロバイダーと共有）
- 広告なし（プライバシー保護の一環として広告を削除）

#### AI/Speech Data Handling
- 音声入力を第三者サービスプロバイダーと共有（音声認識・発音分析）
- 明示的なAI/ML条項はなし

#### Children's Privacy
- 13歳以上を対象としたサービス
- 子供向けに設計されていないため、13歳未満のデータ収集は標準的な成人用プロセス

#### Third-Party Sharing
- 個人情報を第三者に販売・賃貸しない
- マーケティング目的での個人情報共有なし
- 合併・買収・破産の場合に第三者に移転可能性あり

### 3.2 Terms of Service

#### Subscription & Auto-Renewal
- 月額、四半期、半年、年間プランあり
- 更新日の24時間前までにキャンセルしない限り自動更新

### 3.3 Apple App Privacy Labels

#### Data Used to Track You
Identifiers (Device ID)

#### Data Linked to You
- Purchase History, Email, Name
- Photos/Videos, Audio Data, Customer Support
- User ID

#### Data Not Linked to You
- Device ID (Analytics)
- Coarse Location, Device ID, Product Interaction (App Functionality)
- Crash Data (Diagnostics)

**Note**: 競合の中で最もデータ収集が少ない。広告なしのモデルがプライバシーラベルにも反映されている。

---

## 4. JapanesePod101 (Innovative Language Learning)

**Company**: Innovative Language Learning USA LLC (New York, NY / Tokyo office)
**Privacy Policy**: https://www.innovativelanguage.com/privacy
**Terms of Service**: https://www.innovativelanguage.com/terms-of-service

### 4.1 Privacy Policy

#### Data Collected
- **PII**: 名前、年齢、メールアドレス、支払い情報
- **Automatically Collected**: IPアドレス、ブラウザタイプ、OS、閲覧ページ、滞在時間
- **Learning Data**: 学習進捗、アクセスしたレッスン、ダウンロード履歴
- **User Content**: テキスト、音声、データ、画像等を「記録、読取、コピー、開示、使用」する権利を留保（第三者への送信はしない）

#### AI/ML Data Handling
- 明示的なAI/ML条項なし
- ユーザー提出コンテンツをサービス改善目的で処理する権利を留保

#### Children's Privacy
- 13歳未満（米国）または同等年齢（他国）は対象外
- 保護者の同意なく13歳未満が登録した場合、情報と関連アカウントを即座に削除

#### International Data Transfer
- 個人情報は「米国にあるサーバーに安全に送信」される
- EU/スイスの居住者に対するGDPR要件に準拠

#### User Rights
- **GDPR**: アクセス、修正、消去、処理制限、データポータビリティ、異議申立、自動意思決定の制限
- **CCPA**: 収集情報へのアクセス、削除リクエスト、事業目的の共有に関する開示
- 12か月に2回までリクエスト可能、45日以内に回答

#### Data Retention
- 保管目的の達成に必要な期間のみ保持
- 法的遵守や正当なビジネス目的のため一部情報を保持する可能性

#### Third-Party Sharing
- PayPal、Authorize.Net（決済処理）
- Google Analytics、Bing AdWords、Microsoft Clarity、Facebook Pixel（分析）
- Campaigner（マーケティングソフトウェア）
- 「個人情報を第三者に販売または開示しない」と明記（ポリシーに記載された範囲を除く）

#### Cookies
- セッションCookieとパーシステントCookieを使用
- Do Not Track信号には応答しない

### 4.2 Terms of Service

#### Subscription & Auto-Renewal
- 前払い制（期間開始時に支払い）
- 期限切れ後、キャンセルしない限り正規料金で自動更新
- **初回適用の割引・プロモーションは自動更新には適用されない**
- ユーザーが自ら決済プロバイダーでキャンセルする責任

#### Cancellation & Refund
- **60日以内の返金リクエスト**: まず定期課金をキャンセルし、その後60日以内に通知
- キャンセル未実施や60日超過の場合は返金拒否の可能性
- App Store/Google Play経由の場合は各プラットフォームの規約に従う

#### User Content
- **永久的、全世界的、取消不能、ロイヤリティフリー**のライセンスを付与
- 表示、処理、配信、保管、ホスティングに使用可能
- サブライセンス権あり
- ユーザーは知的財産権の所有を保証

#### AI Disclaimers
- AI固有の免責事項なし

#### Liability
- 「AS IS, AS AVAILABLE」で提供
- 損害賠償上限: ユーザーが支払った総額
- 間接的、付随的、特別、懲罰的、結果的損害は免責

### 4.3 Apple App Privacy Labels

#### Data Used to Track You
Identifiers, Usage Data

#### Data Linked to You
- Email Address, Device ID, User ID
- Photos/Videos, Audio Data, Customer Support, Other User Content
- Advertising Data

#### Data Not Linked to You
- Product Interaction (Usage Data)
- Crash Data (Diagnostics)

---

## 5. Best Practices Summary / ベストプラクティスまとめ

### 5.1 Privacy Policy Best Practices

| Practice | Duolingo | Busuu | LingoDeer | JapanesePod101 | Recommendation for myandemy.ai |
|----------|----------|-------|-----------|-----------------|-------------------------------|
| Data categories明確化 | O | O | △ | O | 収集データをカテゴリ別に明確に分類 |
| AI vendor data sharing | O (OpenAI明記) | O (OpenAI, Azure明記) | - | - | **Google Gemini APIとのデータ共有を明記** |
| AI training用データ利用 | △ | O (音声ML訓練を明記) | - | - | AI Tutorの音声・テキストデータの利用範囲を明記 |
| Children's privacy | O (詳細) | △ | △ | O | **17歳以上対象を明記、COPPA準拠** |
| GDPR user rights | O | O | △ | O (詳細) | アクセス・修正・削除・ポータビリティの権利を明記 |
| CCPA compliance | O | △ | - | O (詳細) | California居住者向けの権利セクション |
| Data retention period | △ (曖昧) | △ | - | △ | **具体的な保持期間を明記**（差別化ポイント） |
| International transfer | △ | △ | - | O | Supabase (US)へのデータ転送を明記 |
| Do Not Track対応 | 非対応 | 非対応 | - | 非対応 | 業界標準として非対応を記載 |
| Security measures | △ | O | - | △ | 暗号化、アクセス制御の記載 |
| Social login data | O | O | - | - | Google/Facebook SSO経由のデータ範囲を明記 |

### 5.2 Terms of Service Best Practices

| Practice | Duolingo | Busuu | LingoDeer | JapanesePod101 | Recommendation for myandemy.ai |
|----------|----------|-------|-----------|-----------------|-------------------------------|
| UGC ownership | O (ユーザー保持) | - | - | X (永久ライセンス) | **ユーザーがUGCの所有権を保持**するモデルを推奨 |
| AI disclaimer | △ | △ | - | - | **AI Tutorの回答精度の免責事項を明記** |
| Subscription auto-renewal | O | O | O | O | 24時間前キャンセル、プラットフォーム別の手順 |
| Refund policy | X (返金なし) | △ (初回14日) | - | O (60日) | 初回14日間の返金保証を推奨 |
| Terms change notice | O (1週間前) | - | - | - | 規約変更の事前通知（最低7日）を推奨 |
| Liability cap | - | - | - | O (支払総額) | 損害賠償上限を支払総額に設定 |
| Platform-specific cancellation | O | O | O | O | App Store/Google Play別のキャンセル手順を記載 |

### 5.3 App Store Privacy Labels Best Practices

#### Apple App Privacy Labels - myandemy.ai想定構成

**Data Used to Track You**:
- Identifiers (Device ID) — Google Analytics使用のため
- Usage Data — Analytics目的

**Data Linked to You**:
- Contact Info: Email Address, Name
- Identifiers: User ID, Device ID
- User Content: Audio Data (AI Tutor), Customer Support
- Usage Data: Product Interaction
- Purchases: Purchase History
- Diagnostics: Crash Data, Performance Data

**Data Not Linked to You**:
- Diagnostics: Crash Data (anonymized)
- Usage Data: Product Interaction (aggregated analytics)

**Purpose Mapping**:
| Data Type | Purpose |
|-----------|---------|
| Email, Name | App Functionality, Developer's Marketing |
| User ID | App Functionality, Analytics |
| Device ID | Analytics, Third-Party Advertising (Google Analytics) |
| Audio Data | App Functionality (AI Tutor) |
| Purchase History | App Functionality |
| Product Interaction | Analytics, Product Personalization |
| Crash/Performance Data | App Functionality |

#### Google Play Data Safety - myandemy.ai想定構成

**Data Shared**:
- Device ID, Usage Data → Google Analytics (Analytics purpose)
- Audio/Text Data → Google Gemini API (App Functionality)

**Data Collected**:
- Personal Info: Name, Email
- Financial: Purchase History
- App Activity: Learning progress, in-app actions
- App Info & Performance: Crash logs, diagnostics
- Device/Other IDs: Device ID

**Security Practices**:
- Data encrypted in transit: Yes (HTTPS/TLS)
- Data deletion request: Yes (account deletion)

### 5.4 特定商取引法に基づく表記 Best Practices

語学教室は「特定継続的役務提供」に該当し、特定商取引法の対象。オンラインサブスクリプション形式では以下の項目が必要。

#### 必須記載項目

| 項目 | 記載内容 |
|------|---------|
| 販売業者 | Myandemy Japan合同会社 |
| 運営統括責任者 | 代表者名 |
| 所在地 | 東京都新宿区（番地・建物名まで正確に） |
| 電話番号 | 連絡が取れる実働番号 |
| 電話受付時間 | 例: 平日10:00-18:00 |
| メールアドレス | 問い合わせ用メール |
| URL | https://myandemy.ai (等) |
| 販売価格 | 料金ページ参照、または各プラン金額を明記 |
| 商品代金以外の必要料金 | 消費税等 |
| 支払方法 | クレジットカード、App Store/Google Play内課金 |
| 支払時期 | 購入時即時決済、自動更新時に課金 |
| サービス提供時期 | 決済完了後即時 |
| 返品・キャンセル | デジタルコンテンツの性質上、提供開始後の返品不可（クーリングオフ対象外の旨） |
| 解約方法 | App Store/Google Playでの定期購読キャンセル方法 |
| 契約期間 | 月額/年額プランの契約期間 |
| 自動更新 | 契約期間終了時に自動更新される旨、更新条件 |

#### 2022年改正対応: 最終確認画面の表示義務
サブスクリプション申込時の「最終確認画面」に以下を表示:
- 対価（価格・税込表示）
- 支払時期・方法
- サービス提供時期
- 撤回・解除条件
- 「初回無料」「フリートライアル」等がある場合、定期購入であることを見やすいフォントで明記

---

## 6. myandemy.ai Specific Recommendations / myandemy.ai向け推奨事項

### 6.1 Priority Items

1. **AI Tutor (Gemini API) Data Handling**: Google Gemini APIとの音声・テキストデータ共有を明記。Duolingo/Busuuのモデルを参考に、AIベンダーがデータを保持する可能性について透明性を確保。

2. **Multi-language Privacy Policy**: 日英併記に加え、ミャンマー語・ベトナム語・ネパール語版の検討（少なくとも要約版）。競合はほぼ英語のみだが、myandemy.aiのターゲット層には母語での理解が重要。

3. **Age Restriction**: 17-25歳がターゲットだが、17歳未満のアクセス制限と保護措置を明記。

4. **Supabase Data Location**: データがSupabase (PostgreSQL)に保存されることの開示。サーバー所在地（AWSリージョン等）の明記。

5. **Google Analytics Tracking**: トラッキング目的でのDevice ID使用をApp Storeプライバシーラベルに反映。

### 6.2 Differentiation Opportunities

- **Data Retention明確化**: 競合が曖昧にしている保持期間を具体的に記載（例: アカウント削除後30日以内にデータ完全削除）
- **AI Training Opt-out**: AI Tutorとの会話データをモデル訓練に使用するかどうかの選択権を提供
- **Premium会員の広告データ保護**: Busuuモデルを参考に、有料会員は広告目的のデータ共有なしを明記
- **セキュリティ認証の取得検討**: Busuuが取得しているISO 27001の取得を長期目標に

### 6.3 Legal Compliance Checklist

- [ ] GDPR (EU一般データ保護規則) - ヨーロッパユーザー向け
- [ ] CCPA (カリフォルニア消費者プライバシー法) - 米国ユーザー向け
- [ ] COPPA (児童オンラインプライバシー保護法) - 13歳未満の保護
- [ ] 個人情報保護法 (日本) - 日本国内ユーザー向け
- [ ] 特定商取引法 - サブスクリプションサービスとして
- [ ] Apple App Store Review Guidelines - プライバシーラベル
- [ ] Google Play Data Safety - データ安全セクション
- [ ] PDPA等 (東南アジア各国) - ミャンマー・ベトナム・ネパールユーザー向け

---

## Sources

### Duolingo
- [Privacy Policy](https://www.duolingo.com/privacy)
- [Terms of Service](https://www.duolingo.com/terms)
- [Common Sense Privacy Report](https://privacy.commonsense.org/privacy-report/duolingo)
- [ToS;DR Rating](https://tosdr.org/en/service/744)
- [Duolingo Data Vault (Help Center)](https://support.duolingo.com/hc/en-us/articles/360004256711)
- [App Store Listing](https://apps.apple.com/us/app/duolingo-language-lessons/id570060128)

### Busuu
- [Privacy Policy](https://www.busuu.com/en/privacy)
- [Terms and Conditions](https://www.busuu.com/en/terms)
- [Chegg Privacy Policy](https://www.chegg.com/en-US/privacypolicy)
- [PrivacySpy Rating](https://privacyspy.org/product/busuu/)
- [App Store Listing](https://apps.apple.com/us/app/busuu-language-learning/id379968583)
- [AI Conversation Feature (Press Release)](https://investor.chegg.com/Press-Releases/press-release-details/2024/Busuu-Launches-New-AI-Conversation-Practice-Feature/default.aspx)

### LingoDeer
- [Privacy Policy](https://lingodeer.com/privacypolicy-html)
- [Terms of Service](https://www.lingodeer.com/terms-conditions-html)
- [App Store Listing](https://apps.apple.com/us/app/lingodeer-learn-languages/id1261193709)
- [Common Sense Privacy Evaluation](https://privacy.commonsense.org/evaluation/LingoDeer---Learn-Languages)

### JapanesePod101 / Innovative Language
- [Privacy Policy](https://www.innovativelanguage.com/privacy)
- [Terms of Service](https://www.innovativelanguage.com/terms-of-service)
- [App Store Listing](https://apps.apple.com/us/app/innovative-language-learning/id668386019)

### App Store Guidelines
- [Apple App Privacy Details](https://developer.apple.com/app-store/app-privacy-details/)
- [Google Play Data Safety](https://support.google.com/googleplay/android-developer/answer/10787469)

### 特定商取引法
- [Act on Specified Commercial Transactions (English)](https://www.japaneselawtranslation.go.jp/en/laws/view/3340/en)
- [Consumer Affairs Agency Guide](https://www.no-trouble.caa.go.jp/foreignlanguage/english/)
- [Stripe Guide (Japan)](https://stripe.com/resources/more/specified-commercial-transactions-act-japan)
- [SubscPay Sample Template](https://www.robotpayment.co.jp/service/payment/sample_tokusyouhou/)
- [Online Subscription & 特商法 Analysis](https://www.kottolaw.com/column/230125.html)

### Privacy Analysis
- [Cybernews: Duolingo "Champion of Tracking"](https://cybernews.com/news/duolingo-champion-of-tracking/)
- [NordVPN: Is Duolingo Safe?](https://nordvpn.com/blog/is-duolingo-safe/)
