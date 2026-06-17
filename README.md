# ifLink NEXT — 共創DX人材育成OS

異業種をつなぎ、IF-THEN モジュールで未来を共創するプラットフォーム。
**Premium Edition v2.6 — Mentor Independence Edition**

![hero](assets/images/hero.jpg)

## 🆕 v2.6 で実施した刷新

### 🔄 メンター機能の独立化

| 変更点 | 内容 |
|---|---|
| 共創ビルダー | MENTOR スロット削除 → IF / THEN / ASSET の **3スロット構成** に |
| メンターページ | **3タブの独立機能** として再構築(一覧 / 登録 / AIメンター) |
| カードホルダー | MENTOR 表示を除外、IF/THEN/ASSET のみに集中 |

### 📝 メンタープロフィール登録(新規)

自身の経歴・専門領域・実績を登録して他のメンバーの伴走者になる仕組み:

- **登録項目**: 名前 / 肩書 / 所属 / 専門カテゴリ / タグ / 経歴 / 実績 / 相談テーマ / 相談料 / 連絡手段 / 公開状態
- **AI支援**: 名前と肩書から AI が経歴文を自動補完(API設定時)
- **Myメンターバッジ**: 自身のサイトでは「✨ MY」バッジ + シアン光彩で強調
- **永続化**: LocalStorage で保存、リロード後も維持
- **公開/非公開切替**: 自身のみ閲覧可能なプライベート設定

### 🤖 AIメンター機能(新規)

属性別の **6体のAIメンター** と 24h 対話可能なチャット機能:

| AI | アバター | 専門 | 特徴 |
|---|---|---|---|
| **ビジネス・ストラテジスト** | 💼 | 事業開発 | BCG/McKinseyレベルの思考法、フレームワーク提示 |
| **テクノロジ・アーキテクト** | 🖥️ | 技術 | システム設計・AI/IoT・クラウド・SRE |
| **リーガル・アドバイザー** | ⚖️ | 知財・法務 | NDA・特許・契約・著作権・個人情報保護 |
| **デザイン・UXコーチ** | 🎨 | デザイン | UI/UX・プロダクトデザイン・ブランディング |
| **ファイナンス・コーチ** | 💰 | 資金調達 | VC・Term Sheet・財務モデル・ピッチデック |
| **マインドコーチ** | 🧭 | メンタル | 順心ケア・チームビルディング・コミュニケーション |

#### チャットUI機能

- 💬 **リアルタイムチャット**(タイピングインジケーター付き)
- 🎯 **属性別サジェスト**(よくある相談例ボタン)
- 💾 **会話履歴を永続化**(AIメンター別に保存)
- 🤖 **API連携**: OpenAI / Gemini で実AI対話
- 🎭 **デモ返答**: API未設定時もプロフェッショナルな模擬回答
- 🗑️ **履歴クリア**(AIメンター別)

## ✨ 既存機能(v2.5 から継承)

- 🏠 HOME / ダッシュボード
- 📇 カードホルダー(IF/THEN/ASSET + Myカード)
- 📝 名刺・モジュール登録(AI画像生成 + Myカード化 + 公開ビュー切替)
- ⚡ 共創ビルダー(IF×THEN×ASSET の3スロットで PoC 自動生成)
- 🛒 マーケットプレイス
- 🌐 共創共有 / コミュニティ
- 📊 分析・レポート
- 💎 プレミアム機能
- 🌐 多言語(日 / 英 / 中)
- 💾 LocalStorage 永続化
- 🤖 OpenAI / Gemini API 連携
- 🔍 SEO + OGP + Favicon + 404 + manifest

## 🎬 動作シナリオ

### メンタープロフィール登録
1. 「メンター」→ 「📝 メンタープロフィール登録」タブ
2. 名前・肩書を入力 → 「🤖 AIで経歴文を補完」
3. 実績・テーマ・相談料・連絡手段を記入
4. 「✨ プロフィールを登録・保存」 (+80pt)
5. 一覧タブで自身のプロフィールがシアン光彩で表示

### AIメンター壁打ち
1. 「メンター」→ 「🤖 AIメンター」タブ
2. 6体から専門分野に合うAIメンターを選択
3. サジェストから質問を選ぶか、自由入力
4. Cmd/Ctrl + Enter で送信
5. 履歴は自動保存 → 別のAIメンターに切替後、戻ると会話再開可

## 📁 ファイル構成

```
.
├── index.html                      # メインアプリ (161.3KB)
├── 404.html
├── manifest.webmanifest
├── robots.txt / sitemap.xml
├── favicon.ico
├── README.md
├── .nojekyll / .gitignore
├── .github/workflows/deploy.yml    # GitHub Actions 自動デプロイ
└── assets/images/                  # 画像 (2.7MB / WebP+JPEG)
```

## 🚀 GitHub Pages 公開手順

```bash
unzip iflink-next-v2.6.zip
cd iflink-next-v2.6
git init && git add . && git commit -m "v2.6 Mentor Independence"
git branch -M main
git remote add origin https://github.com/<user>/<repo>.git
git push -u origin main
```

UI: **Settings → Pages → Source: `GitHub Actions`** で自動デプロイ。

## 🛠 ローカル動作確認

```bash
python3 -m http.server 8000
# → http://localhost:8000/
```

---

**© 2026 ifLink NEXT — IF-THEN Innovation OS / Mentor Independence Edition**
