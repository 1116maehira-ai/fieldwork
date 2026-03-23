# SALES ENGINE — 広告代理店向け営業支援ツール

> アタックリスト管理からアポ獲得・商談・受注まで一貫して管理できる営業支援システム

🔗 **ライブURL**: https://1116maehira-ai.github.io/fieldwork/

---

## ツール構成

| ツール | 役割 | URL |
|---|---|---|
| **FIELDWORK** | 情報収集 → アプローチ → アポ獲得 | `/fieldwork.html` |
| **DEALWORK** | 商談 → 提案 → 受注 | `/dealwork.html` |

---

## 主な機能

### FIELDWORK
- AIスコアリング（予算ポテンシャル・緊急度・アプローチ適性の3軸）
- アタックリスト管理（S/A/B/Cランク）
- アプローチ自動フェーズ管理（訪問→電話→手紙→冷却期間のループ）
- 次のアクション日程を自動計算（土日祝スキップ・JST対応）
- 直筆手紙AI作成（HP・SNSスキャン→トピックス抽出→文章生成）
- 手紙送付依頼管理

### DEALWORK
- 商談ヒアリングシート（ボタン選択式・書かない設計）
- 商談入り方3パターン（プッシュ型 / 課題型 / ソリューション決定済み）
- 提案書サマリー自動生成（沖縄県相場データ内蔵）
- 商談パイプライン管理（ヒアリング→提案→クロージング→受注）
- 受注・失注ダッシュボード

---

## 技術スタック

- **フロントエンド**: Vanilla HTML / CSS / JavaScript（フレームワークなし）
- **ホスティング**: GitHub Pages
- **フォント**: Bebas Neue / Noto Sans JP / JetBrains Mono（Google Fonts）
- **データ保存**: window.storage API（セッション内）/ Supabase（予定）
- **AI機能**: Anthropic Claude API（手紙生成・情報スキャン）

---

## 今後の実装予定

- [ ] Google Maps API連携（業種×エリアで企業を自動収集）
- [ ] 求人ボックスAPI連携（求人中企業を成長シグナルとして検出）
- [ ] Supabaseでのデータ永続化
- [ ] Google Apps Script経由でのAPIキー安全管理
- [ ] お名前.comの独自ドメイン設定

---

## ファイル構成

```
fieldwork/
├── index.html        # トップページ（ツール選択）
├── fieldwork.html    # アタック→アポ獲得ツール
├── dealwork.html     # 商談→受注ツール
└── README.md         # このファイル
```

---

## GitHub Pages 設定方法

1. Settings → Pages
2. Source: `Deploy from a branch`
3. Branch: `main` / `/ (root)`
4. Save → URLが発行される

---

*Built for ad agency sales teams in Okinawa, Japan*
