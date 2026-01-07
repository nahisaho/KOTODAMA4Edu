# KOTODAMA - Interactive Agentic Prompt Templates

<p align="center">
  <strong>🎯 AIを専門家として機能させるための対話型プロンプトテンプレート集</strong>
</p>

<p align="center">
  <a href="#特徴">特徴</a> •
  <a href="#テンプレート一覧">テンプレート一覧</a> •
  <a href="#使い方">使い方</a> •
  <a href="#ドキュメント">ドキュメント</a> •
  <a href="#ライセンス">ライセンス</a>
</p>


## 概要

**KOTODAMA**は、AIが能動的に対話を主導し、段階的に文脈を収集しながら、理論・フレームワークに基づいた専門的な提案を生成するための**Interactive Agentic Prompt（IAP）** テンプレート集です。

従来のプロンプトとは異なり、AIが「一問一答」形式で質問を投げかけ、ユーザーの状況を深く理解した上で、専門家レベルの回答を提供します。

### 📦 テンプレートバリエーション

| バージョン | 用途 |
|------------|------|
| **フル版** (`templates/full/`) | 詳細な理論・フレームワークを含む完全版（約13,000文字） |
| **LLM最適化版** | 各LLMの特性に合わせて最適化（下記参照） |

### 🤖 LLM最適化版

各LLMの特性に合わせて最適化されたプロンプトを提供しています。

| LLM | ディレクトリ | 最適化特徴 |
|-----|-------------|-----------|
| **GPT-4o/5** | `templates/gpt/` | 英語System Prompt見出し、IMPORTANT REMINDERS、推奨パラメータ設定 |
| **Claude 4.x** | `templates/claude/` | XMLタグ構造化、Extended Thinking活用ガイド、Claude Projects連携 |
| **MS Copilot** | `templates/copilot/` | Role and Purpose見出し、M365 Integration Tips、KEY REMINDERS |
| **Gemini Pro** | `templates/gemini/` | 太字見出し形式、Critical Rules、Google Workspace連携 |

> 💡 **推奨**: お使いのLLMに対応した最適化版を使用することで、より効果的な対話が可能です。

## 特徴

### 🔄 Interactive（対話的）
- AIが一問一答形式で能動的に質問を投げかけます
- 認知負荷とワーキングメモリを考慮した設計
- 選択肢の提示で回答しやすく

### 🤖 Agentic（エージェント的）
- AIが自律的に判断し、最適な理論・手法を選択
- 5フェーズアーキテクチャで体系的なプロセス
- メタプロンプト生成による動的な最適化

### 📚 理論・フレームワーク統合
- 各専門分野の理論を体系的に組み込み
- 根拠のある専門的な提案を生成
- 再現性の高い回答

### ✨ 回答品質強化（v1.1）
- **思考チェーン（Chain of Thought）**: AIの内部思考プロセスを明示化
- **出力品質チェックリスト**: 専門的・倫理的観点を網羅
- **エラー回復プロンプト**: 対話が行き詰まった場合の回復手順
- **回答の深さ調整ガイド**: 簡潔/詳細な回答の使い分け
- **AIモデル別適用ガイド**: Microsoft 365 Copilot/ChatGPT/Claude/Gemini対応

## テンプレート一覧

全**41種類**のテンプレートを提供しています。

### 学校現場系（23種類）

| カテゴリ | テンプレート |
|---------|-------------|
| **教育・授業** | [教育者](templates/full/educator-interactive-agentic-prompt.md)、[国語科指導](templates/full/japanese-language-instructor-interactive-agentic-prompt.md)、[道徳教育](templates/full/moral-education-coordinator-interactive-agentic-prompt.md)、[カリキュラム](templates/full/curriculum-coordinator-interactive-agentic-prompt.md)、[特別活動](templates/full/special-activities-coordinator-interactive-agentic-prompt.md) |
| **生徒支援** | [生徒指導](templates/full/student-guidance-interactive-agentic-prompt.md)、[学習カウンセラー](templates/full/learning-counselor-interactive-agentic-prompt.md)、[スクールカウンセラー](templates/full/school-counselor-interactive-agentic-prompt.md)、[スクールソーシャルワーカー](templates/full/school-social-worker-interactive-agentic-prompt.md)、[進路指導](templates/full/career-counselor-interactive-agentic-prompt.md)、[学校間連携](templates/full/school-transition-coordinator-interactive-agentic-prompt.md) |
| **特別支援** | [特別支援コーディネーター](templates/full/special-needs-coordinator-interactive-agentic-prompt.md) |
| **健康・安全** | [養護教諭](templates/full/school-nurse-interactive-agentic-prompt.md)、[栄養教諭](templates/full/nutrition-teacher-interactive-agentic-prompt.md)、[安全・防災](templates/full/safety-disaster-coordinator-interactive-agentic-prompt.md) |
| **学校運営** | [学校管理者](templates/full/school-administrator-interactive-agentic-prompt.md)、[学年主任](templates/full/grade-leader-interactive-agentic-prompt.md)、[部活動顧問](templates/full/club-activity-advisor-interactive-agentic-prompt.md)、[保護者対応](templates/full/parent-relations-interactive-agentic-prompt.md)、[施設管理](templates/full/school-facilities-manager-interactive-agentic-prompt.md)、[学校司書](templates/full/school-librarian-interactive-agentic-prompt.md) |
| **ICT** | [ICT教育](templates/full/ict-education-coordinator-interactive-agentic-prompt.md)、[EdTech DXコンサルタント](templates/full/edtech-dx-consultant-interactive-agentic-prompt.md) |

### 教育行政系（9種類）

| カテゴリ | テンプレート |
|---------|-------------|
| **行政** | [教育長](templates/full/superintendent-interactive-agentic-prompt.md)、[教育委員会](templates/full/board-of-education-interactive-agentic-prompt.md)、[人事管理](templates/full/personnel-administrator-interactive-agentic-prompt.md) |
| **指導主事** | [学校教育指導主事](templates/full/school-supervisor-interactive-agentic-prompt.md)、[生徒指導指導主事](templates/full/student-guidance-supervisor-interactive-agentic-prompt.md)、[特別支援指導主事](templates/full/special-needs-supervisor-interactive-agentic-prompt.md) |
| **その他** | [教育センター](templates/full/education-center-interactive-agentic-prompt.md)、[社会教育](templates/full/social-education-coordinator-interactive-agentic-prompt.md)、[教師メンター](templates/full/teacher-mentor-interactive-agentic-prompt.md) |

### 高等教育系（9種類） 🆕

| カテゴリ | テンプレート |
|---------|-------------|
| **教育・研究** | [大学教員](templates/full/university-faculty-interactive-agentic-prompt.md)、[研究指導者](templates/full/research-supervisor-interactive-agentic-prompt.md)、[FD担当者](templates/full/faculty-developer-interactive-agentic-prompt.md) |
| **学生支援** | [キャリア支援](templates/full/university-career-support-interactive-agentic-prompt.md)、[留学生支援](templates/full/international-student-support-interactive-agentic-prompt.md)、[学生相談](templates/full/university-student-counselor-interactive-agentic-prompt.md) |
| **大学運営** | [学部長・学科長](templates/full/academic-department-head-interactive-agentic-prompt.md)、[産学連携コーディネーター](templates/full/industry-academia-coordinator-interactive-agentic-prompt.md)、[入試広報担当](templates/full/admissions-officer-interactive-agentic-prompt.md) |

## 各テンプレートの詳細説明

### 🎓 教育・授業系

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[教育者](templates/full/educator-interactive-agentic-prompt.md)**<br>`educator-interactive-agentic-prompt.md` | 授業設計・教育計画を立てたい | 授業設計、教材開発、学習活動設計、評価方法の検討 |
| **[国語科指導](templates/full/japanese-language-instructor-interactive-agentic-prompt.md)**<br>`japanese-language-instructor-interactive-agentic-prompt.md` | 国語の指導方法を改善したい | 読解指導、作文指導、文法指導、言語活動の設計 |
| **[道徳教育](templates/full/moral-education-coordinator-interactive-agentic-prompt.md)**<br>`moral-education-coordinator-interactive-agentic-prompt.md` | 道徳の授業を充実させたい | 道徳授業の設計、価値の明確化、議論の活性化 |
| **[カリキュラム](templates/full/curriculum-coordinator-interactive-agentic-prompt.md)**<br>`curriculum-coordinator-interactive-agentic-prompt.md` | 教育課程の編成・改善をしたい | カリキュラム・マネジメント、教科横断的な学習、評価計画 |
| **[特別活動](templates/full/special-activities-coordinator-interactive-agentic-prompt.md)**<br>`special-activities-coordinator-interactive-agentic-prompt.md` | 学校行事や生徒会活動を活性化したい | 学校行事の企画、生徒会活動、学級活動の設計 |

### 👥 生徒支援系

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[生徒指導](templates/full/student-guidance-interactive-agentic-prompt.md)**<br>`student-guidance-interactive-agentic-prompt.md` | 生徒の問題行動やいじめに対応したい | 問題行動への対応、いじめ対応、不登校支援、規律指導 |
| **[学習カウンセラー](templates/full/learning-counselor-interactive-agentic-prompt.md)**<br>`learning-counselor-interactive-agentic-prompt.md` | 学習に困難を抱える生徒を支援したい | 学習方法の改善、学習意欲の向上、学習困難への対応 |
| **[スクールカウンセラー](templates/full/school-counselor-interactive-agentic-prompt.md)**<br>`school-counselor-interactive-agentic-prompt.md` | 心理的支援が必要な生徒がいる | 心理アセスメント、カウンセリング、危機介入、教員へのコンサルテーション |
| **[スクールソーシャルワーカー](templates/full/school-social-worker-interactive-agentic-prompt.md)**<br>`school-social-worker-interactive-agentic-prompt.md` | 家庭環境に課題がある生徒を支援したい | 福祉機関との連携、家庭支援、虐待対応、貧困支援 |
| **[進路指導](templates/full/career-counselor-interactive-agentic-prompt.md)**<br>`career-counselor-interactive-agentic-prompt.md` | 生徒の進路選択を支援したい | 進路相談、キャリア教育、進学・就職指導、保護者連携 |
| **[学校間連携](templates/full/school-transition-coordinator-interactive-agentic-prompt.md)**<br>`school-transition-coordinator-interactive-agentic-prompt.md` | 小中連携・中高連携を強化したい | 学校間の情報共有、接続期の支援、連携カリキュラム |

### 🤝 特別支援系

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[特別支援コーディネーター](templates/full/special-needs-coordinator-interactive-agentic-prompt.md)**<br>`special-needs-coordinator-interactive-agentic-prompt.md` | 特別な支援が必要な児童生徒を支援したい | IEP作成、合理的配慮、通級指導、保護者支援、関係機関連携 |

### 🏥 健康・安全系

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[養護教諭](templates/full/school-nurse-interactive-agentic-prompt.md)**<br>`school-nurse-interactive-agentic-prompt.md` | 児童生徒の心身の健康を守りたい | 健康管理、保健室経営、健康教育、メンタルヘルス、感染症対策 |
| **[栄養教諭](templates/full/nutrition-teacher-interactive-agentic-prompt.md)**<br>`nutrition-teacher-interactive-agentic-prompt.md` | 食育を推進したい | 食育指導、給食管理、アレルギー対応、栄養教育 |
| **[安全・防災](templates/full/safety-disaster-coordinator-interactive-agentic-prompt.md)**<br>`safety-disaster-coordinator-interactive-agentic-prompt.md` | 学校の安全・防災体制を強化したい | 防災計画、避難訓練、安全教育、危機管理 |

### 🏫 学校運営系

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[学校管理者](templates/full/school-administrator-interactive-agentic-prompt.md)**<br>`school-administrator-interactive-agentic-prompt.md` | 学校経営の課題を解決したい | 学校運営、教職員マネジメント、危機管理、地域連携 |
| **[学年主任](templates/full/grade-leader-interactive-agentic-prompt.md)**<br>`grade-leader-interactive-agentic-prompt.md` | 学年経営を改善したい | 学年経営、担任支援、学年行事、保護者対応 |
| **[部活動顧問](templates/full/club-activity-advisor-interactive-agentic-prompt.md)**<br>`club-activity-advisor-interactive-agentic-prompt.md` | 部活動運営の悩みを解決したい | 部活動運営、生徒指導、保護者対応、働き方改革 |
| **[保護者対応](templates/full/parent-relations-interactive-agentic-prompt.md)**<br>`parent-relations-interactive-agentic-prompt.md` | 保護者との関係構築を強化したい | クレーム対応、保護者会、連携強化、困難ケース対応 |
| **[施設管理](templates/full/school-facilities-manager-interactive-agentic-prompt.md)**<br>`school-facilities-manager-interactive-agentic-prompt.md` | 学校施設の管理・改善をしたい | 施設管理、環境整備、安全管理、修繕計画 |
| **[学校司書](templates/full/school-librarian-interactive-agentic-prompt.md)**<br>`school-librarian-interactive-agentic-prompt.md` | 学校図書館を活性化したい | 図書館運営、読書推進、情報リテラシー教育、授業支援 |

### 💻 ICT・DX系

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[ICT教育](templates/full/ict-education-coordinator-interactive-agentic-prompt.md)**<br>`ict-education-coordinator-interactive-agentic-prompt.md` | GIGAスクール・ICT活用を推進したい | ICT活用授業、情報モラル教育、GIGAスクール推進 |
| **[EdTech DXコンサルタント](templates/full/edtech-dx-consultant-interactive-agentic-prompt.md)**<br>`edtech-dx-consultant-interactive-agentic-prompt.md` | 教育DXを戦略的に進めたい | DX戦略、システム導入、組織変革、教職員研修 |

### 🏛️ 教育行政系

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[教育長](templates/full/superintendent-interactive-agentic-prompt.md)**<br>`superintendent-interactive-agentic-prompt.md` | 教育行政のトップとしてビジョンを策定したい | 教育ビジョン、教育振興計画、首長・議会連携、組織マネジメント |
| **[教育委員会](templates/full/board-of-education-interactive-agentic-prompt.md)**<br>`board-of-education-interactive-agentic-prompt.md` | 教育政策の立案・実施をしたい | 教育政策、学校支援・指導、教職員人事・研修、地域連携 |
| **[人事管理](templates/full/personnel-administrator-interactive-agentic-prompt.md)**<br>`personnel-administrator-interactive-agentic-prompt.md` | 教職員の人事管理を行いたい | 人事異動、採用、評価、服務管理、働き方改革 |
| **[学校教育指導主事](templates/full/school-supervisor-interactive-agentic-prompt.md)**<br>`school-supervisor-interactive-agentic-prompt.md` | 学校の教育活動を指導・支援したい | 授業改善指導、研修企画、教育課程指導、学校訪問 |
| **[生徒指導指導主事](templates/full/student-guidance-supervisor-interactive-agentic-prompt.md)**<br>`student-guidance-supervisor-interactive-agentic-prompt.md` | 管内の生徒指導を統括したい | いじめ・不登校対策、生徒指導体制、危機対応 |
| **[特別支援指導主事](templates/full/special-needs-supervisor-interactive-agentic-prompt.md)**<br>`special-needs-supervisor-interactive-agentic-prompt.md` | 特別支援教育を推進したい | 特別支援教育体制、インクルーシブ教育、研修企画 |
| **[教育センター](templates/full/education-center-interactive-agentic-prompt.md)**<br>`education-center-interactive-agentic-prompt.md` | 教職員研修や調査研究を行いたい | 研修企画・運営、教育相談、調査研究、教材開発 |
| **[社会教育](templates/full/social-education-coordinator-interactive-agentic-prompt.md)**<br>`social-education-coordinator-interactive-agentic-prompt.md` | 社会教育・生涯学習を推進したい | 公民館活動、生涯学習、地域学校協働、青少年教育 |
| **[教師メンター](templates/full/teacher-mentor-interactive-agentic-prompt.md)**<br>`teacher-mentor-interactive-agentic-prompt.md` | 新任・若手教員を育成したい | 初任者指導、OJT、授業力向上、メンタルヘルス |

### 🎓 高等教育系 🆕

| テンプレート | こんな時に使う | 主な相談内容 |
|-------------|---------------|-------------|
| **[大学教員](templates/full/university-faculty-interactive-agentic-prompt.md)**<br>`university-faculty-interactive-agentic-prompt.md` | 大学の授業・講義を改善したい | 授業設計、アクティブラーニング、成績評価、オンライン授業 |
| **[研究指導者](templates/full/research-supervisor-interactive-agentic-prompt.md)**<br>`research-supervisor-interactive-agentic-prompt.md` | ゼミ・大学院生の研究指導を充実させたい | ゼミ運営、論文指導、研究倫理、院生のメンタルヘルス |
| **[FD担当者](templates/full/faculty-developer-interactive-agentic-prompt.md)**<br>`faculty-developer-interactive-agentic-prompt.md` | 教員の授業改善を組織的に支援したい | FD研修企画、授業コンサルテーション、教育改善 |
| **[キャリア支援](templates/full/university-career-support-interactive-agentic-prompt.md)**<br>`university-career-support-interactive-agentic-prompt.md` | 大学生の就職・キャリア形成を支援したい | キャリア相談、就活支援、キャリア教育、企業連携 |
| **[留学生支援](templates/full/international-student-support-interactive-agentic-prompt.md)**<br>`international-student-support-interactive-agentic-prompt.md` | 留学生の学習・生活を支援したい | 異文化適応、日本語支援、就職支援、交流促進 |
| **[学生相談](templates/full/university-student-counselor-interactive-agentic-prompt.md)**<br>`university-student-counselor-interactive-agentic-prompt.md` | 大学生のメンタルヘルスを支援したい | 心理相談、発達障害支援、危機対応、合理的配慮 |
| **[学部長・学科長](templates/full/academic-department-head-interactive-agentic-prompt.md)**<br>`academic-department-head-interactive-agentic-prompt.md` | 学部・学科の運営を改善したい | 組織運営、カリキュラム改革、教員マネジメント、認証評価 |
| **[産学連携コーディネーター](templates/full/industry-academia-coordinator-interactive-agentic-prompt.md)**<br>`industry-academia-coordinator-interactive-agentic-prompt.md` | 産学連携・研究協力を推進したい | 共同研究、知財管理、技術移転、スタートアップ支援 |
| **[入試広報担当](templates/full/admissions-officer-interactive-agentic-prompt.md)**<br>`admissions-officer-interactive-agentic-prompt.md` | 学生募集・入試広報を強化したい | 志願者確保、広報戦略、オープンキャンパス、高大連携 |

## 使い方

### 1. テンプレートの選択

あなたの役割や相談内容に合ったテンプレートを選択します。

### 2. AIへの貼り付け

テンプレートの内容をコピーし、お使いのAIツールに貼り付けます。

> ⚠️ **重要**: テンプレートをコピーする際は、**ヘッダー部分**（`> 📅 作成日:` など）と**フッター部分**（ライセンス表記など）を削除してください。本文の `# ロール定義` または `# Role and Purpose` から始めてコピーしてください。

| AIモデル | 推奨設定 |
|---------|---------|
| **ChatGPT (GPT-4)** | Custom Instructionsに追記、または会話冒頭に貼り付け |
| **Claude** | プロンプト全文を会話冒頭に貼り付け（長文コンテキスト得意） |
| **Gemini** | 構造化して提示 |

### 3. 対話の開始

AIが最初の質問を投げかけます。選択肢から選ぶか、自由に回答してください。

### 4. 段階的な対話

AIが段階的に質問を重ね、あなたの状況を深く理解していきます。

### 5. 専門的な提案の受け取り

収集した情報と適切な理論に基づいた、具体的で実行可能な提案を受け取ります。

## ドキュメント

- [Interactive Agentic Prompt 完全ガイド](docs/interactive-agentic-prompt-guide.md) - 設計思想から実装方法まで包括的に解説
- [IAP作成マニフェスト](docs/iap-creation-manifest.md) - 他分野向けIAPを作成するための設計指針 🆕

## プロジェクト構造

```
KOTODAMA/
├── README.md                 # このファイル
├── CHANGELOG.md              # 変更履歴
├── AGENTS.md                 # エージェント設定
├── docs/
│   ├── interactive-agentic-prompt-guide.md  # 完全ガイド
│   └── iap-creation-manifest.md             # IAP作成マニフェスト
├── steering/                 # プロジェクト設定
│   ├── product.md
│   ├── structure.md
│   ├── tech.md
│   └── rules/
│       └── constitution.md
└── templates/                # 41種類のIAPテンプレート
    ├── full/                 # フル版（詳細版）
    ├── gpt/                  # GPT最適化版
    ├── claude/               # Claude最適化版
    ├── copilot/              # Copilot最適化版
    └── gemini/               # Gemini最適化版
```

## 5フェーズアーキテクチャ

各テンプレートは以下の5フェーズで構成されています。

```
Phase 1 (Discovery) → Phase 2 (Context Gathering) → Phase 3 (SKILL Selection) → Phase 4 (Meta-Prompt Generation) → Phase 5 (Response Generation)
```

| Phase | 名称 | 目的 |
|-------|------|------|
| 1 | Discovery | 真のニーズを発見する |
| 2 | Context Gathering | 状況を多角的に把握する |
| 3 | SKILL Selection | 最適な理論・手法を選ぶ |
| 4 | Meta-Prompt Generation | 専門家としての指示を生成 |
| 5 | Response Generation | 価値ある提案を出力 |

## バージョン履歴

| バージョン | 日付 | 変更内容 |
|-----------|------|----------|
| v1.4 | 2026-01-07 | LLM最適化版を追加（GPT/Claude/Copilot/Gemini各41テンプレート、計164ファイル）。コンパクト版を廃止しLLM最適化版に置換 |
| v1.3 | 2025-12-22 | ディレクトリ構造を`full/`・`compact/`に再編成（v1.4でcompactは廃止） |
| v1.2 | 2025-12-22 | 高等教育系テンプレート9種類を追加（大学教員、研究指導者、FD担当者、キャリア支援、留学生支援、学生相談、学部長・学科長、産学連携、入試広報）。全41テンプレートに拡充 |
| v1.1 | 2025-12-21 | 全32テンプレートに回答品質強化セクション・AIモデル別適用ガイドを追加 |
| v1.0 | 2025-12-20 | 初回リリース（32種類のテンプレート） |

詳細な変更履歴は [CHANGELOG.md](CHANGELOG.md) をご覧ください。

## 貢献

プルリクエストや Issue は歓迎します。新しいテンプレートの提案や既存テンプレートの改善にご協力ください。

## ライセンス

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

このプロジェクトは [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/) の下で公開されています。

- ✅ 非営利目的での使用・改変・再配布が可能
- ✅ クレジット表示が必要
- ❌ 商用利用は禁止

商用利用をご希望の場合は、著作権者にお問い合わせください。

---

<p align="center">
  <strong>KOTODAMAで、AIを真の専門家パートナーに。</strong>
</p>
