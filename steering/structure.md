# Project Structure

**Project**: InteractiveAgenticPrompts (KOTODAMA)
**Last Updated**: 2025-12-22
**Version**: 1.5

---

## Architecture Pattern

**Primary Pattern**: ドキュメントベース・テンプレートリポジトリ

> 本プロジェクトは、教育現場向けInteractive Agentic Promptテンプレートの集約リポジトリです。
> Markdown形式のテンプレートとドキュメンテーションを中心に構成されています。

---

## Directory Organization

### Root Structure

```
InteractiveAgenticPrompts/
├── docs/                     # ドキュメンテーション
│   ├── interactive-agentic-prompt-guide.md  # IAPガイド記事
│   ├── iap-creation-manifest.md             # IAP作成マニフェスト
│   └── Wrighting_Qiita.md                    # Qiita記事下書き
├── templates/                # IAPテンプレート集（41種類）
│   ├── full/                 # フル版（詳細版・約13,000文字）
│   │   ├── educator-interactive-agentic-prompt.md
│   │   ├── learning-counselor-interactive-agentic-prompt.md
│   │   ├── ... (全41ファイル)
│   │   └── university-student-counselor-interactive-agentic-prompt.md
│   └── compact/              # コンパクト版（8,000文字以内）
│       ├── educator-interactive-agentic-prompt.md
│       ├── learning-counselor-interactive-agentic-prompt.md
│       ├── ... (全41ファイル)
│       └── university-student-counselor-interactive-agentic-prompt.md
├── storage/                  # SDD成果物
│   ├── specs/                # 要件・設計・タスク
│   ├── changes/              # 変更仕様
│   └── features/             # 機能仕様
├── steering/                 # プロジェクトメモリ
│   ├── structure.md          # 本ファイル
│   ├── tech.md               # 技術スタック
│   ├── product.md            # プロダクトコンテキスト
│   └── rules/                # ガバナンス
│       └── constitution.md   # 憲法
├── AGENTS.md                 # エージェント設定
└── README.md                 # プロジェクトREADME
```

---

## Template Structure

各IAPテンプレートは統一された5フェーズ構造に従います：

### IAP Template Structure

```markdown
# Interactive Agentic Prompt for [Role]

## System Prompt
[エージェントの役割定義]

## Phase 1: Discovery Phase
[深掘り質問フレームワーク]

## Phase 2: Context Gathering Phase
[必須収集項目、質問例]

## Phase 3: SKILL Selection Phase
[理論・フレームワークリポジトリ]

## Phase 4: Meta-Prompt Generation
[メタプロンプトテンプレート]

## Phase 5: Response Generation
[出力フォーマット]

## 回答品質強化セクション
[思考チェーン、品質チェックリスト、エラー回復プロンプト]

## AIモデル別適用ガイド
[ChatGPT/Claude/Gemini向けガイド]

## Phase 5: Response Generation
[出力フォーマット]

## 理論選択ガイドライン
[課題別推奨理論マトリクス]

## 使用例
[具体的な対話例]

## 注意事項
[緑急対応、リスク管理]
```

---

## Template Categories

### 教育・学習支援系（8種類）

| テンプレート | 対象者 | 主な理論・フレームワーク |
|--------------|--------|------------------------|
| educator | 教員 | UbD, ブルームのタキソノミー, UDL |
| learning-counselor | 学習支援 | メタ認知, 自己調整学習 |
| special-needs-coordinator | 特別支援 | 個別の指導計画, 合理的配慮 |
| school-librarian | 司書教諭 | 情報リテラシー, Big6 |
| curriculum-coordinator | カリキュラムコーディネーター | カリキュラムマネジメント |
| moral-education-coordinator | 道徳教育コーディネーター | 道徳科の評価, 議論する道徳 |
| ict-education-coordinator | ICT教育コーディネーター | SAMR, TPACK, GIGAスクール |
| japanese-language-instructor | 日本語指導担当 | JSL, CLD児童生徒支援 |

### 生徒指導・相談系（7種類）

| テンプレート | 対象者 | 主な理論・フレームワーク |
|--------------|--------|------------------------|
| student-guidance | 生徒指導 | PBS, 修復的実践, FBA |
| career-counselor | 進路指導 | Holland, Super, ナラティブ |
| school-nurse | 養護教諭 | ヘルスプロモーション, TIC |
| school-counselor | スクールカウンセラー | 来談者中心, CBT, 解決志向 |
| school-social-worker | スクールソーシャルワーカー | エコロジカル, 社会資源連携 |
| nutrition-teacher | 栄養教諭 | 食育, アレルギー対応 |
| school-transition-coordinator | 進学・接続コーディネーター | スタートカリキュラム, 接続期 |

### マネジメント・連携系（5種類）

| テンプレート | 対象者 | 主な理論・フレームワーク |
|--------------|--------|------------------------|
| school-administrator | 管理職 | 学習する組織, Kotterの8ステップ |
| grade-leader | 学年主任 | チームビルディング, 心理的安全性 |
| teacher-mentor | メンター | OJT, コーチング |
| parent-relations | 保護者対応 | LEARN法, クレーム対応 |
| personnel-administrator | 人事管理者 | 人材育成, 評価制度 |

### 安全・環境系（3種類）

| テンプレート | 対象者 | 主な理論・フレームワーク |
|--------------|--------|------------------------|
| safety-disaster-coordinator | 安全・防災コーディネーター | 危機管理, BCP, 避難訓練 |
| school-facilities-manager | 施設管理者 | ファシリティマネジメント |
| special-activities-coordinator | 特別活動コーディネーター | 特別活動, 学校行事 |

### 部活・課外活動系（1種類）

| テンプレート | 対象者 | 主な理論・フレームワーク |
|--------------|--------|------------------------|
| club-activity-advisor | 部活顧問 | コーチング, メンタルスキル |

### 教育行政系（9種類）

| テンプレート | 対象者 | 主な理論・フレームワーク |
|--------------|--------|------------------------|
| board-of-education | 教育委員会 | 教育行政, 政策立案 |
| education-center | 教育センター | 研修設計, 教員育成 |
| school-supervisor | 指導主事 | 学校訪問, 授業改善 |
| special-needs-supervisor | 特別支援指導主事 | 特別支援教育政策 |
| student-guidance-supervisor | 生徒指導主事 | 生徒指導政策, 連携体制 |
| social-education-coordinator | 社会教育コーディネーター | 生涯学習, 地域連携 |
| superintendent | 教育長 | 教育ビジョン, 組織運営 |
| edtech-dx-consultant | EdTech DXコンサルタント | SAMR, TPACK, DX推進 |

---

## Design Guidelines

### ドキュメントベースプロジェクトの原則

- **コード不要**: 本プロジェクトはMarkdownテンプレートのリポジトリ
- **一貫した構造**: 全テンプレートが5フェーズ構造に従う
- **拡張可能**: 新しい専門領域のテンプレートを追加可能

---

## SDD Artifacts Organization

### Storage Directory

```
storage/
├── specs/                # 要件・設計・タスク
│   └── [feature]-requirements.md
├── changes/              # 変更仕様
│   └── [change]-spec.md
└── features/             # 機能仕様
    └── [feature].json
```

---

## Documentation Organization

### ドキュメント構造

```
docs/
├── interactive-agentic-prompt-guide.md  # IAPガイド記事
└── Wrighting_Qiita.md                    # Qiita記事下書き
```

---

## Naming Conventions

### ファイル命名規約

- **テンプレート**: `[role]-interactive-agentic-prompt.md`
  - 例: `educator-interactive-agentic-prompt.md`
- **ドキュメント**: `kebab-case.md`
- **Steering**: `[category].md`

### ディレクトリ命名規約

- **英語**: `kebab-case`
- **機能別**: 目的を明確に表す名前

---

## Version Control

### Branch Organization

- `main` - Production branch（公開版）
- `develop` - Development branch（開発版）
- `feature/*` - Feature branches（新テンプレート開発）
- `docs/*` - Documentation branches（ドキュメント更新）

### Commit Message Convention

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types**:
- `feat`: 新しいテンプレート追加
- `fix`: テンプレート修正
- `docs`: ドキュメント更新
- `chore`: その他のメンテナンス

**Example**:

```
feat(templates): 栄養教諭テンプレートを追加

nutrition-teacher-interactive-agentic-prompt.md を新規作成。
食育、アレルギー対応の理論・フレームワークを含む。
```

---

## Changelog

### Version 1.5 (2025-12-22)

- テンプレートを full/ と compact/ の2ディレクトリ構成に変更
- コンパクト版（8,000文字以内）41ファイルを追加
- 高等教育系テンプレート9種類を追加（計41種類）
- IAP作成マニフェストをdocs/に追加

### Version 1.4 (2025-12-21)

- ルートディレクトリにREADME.mdを追加
- プロジェクト名をKOTODAMAとして明示
- ドキュメント構造を更新

### Version 1.3 (2025-12-21)

- IAP Template Structureに回答品質強化セクションを追加
- IAP Template StructureにAIモデル別適用ガイドを追加
- 全テンプレートをv1.1に更新

### Version 1.2 (2025-12-21)

- ディレクトリ構造を32種類のテンプレートに対応
- Template Categories を6カテゴリに再編成
- 不要なコードプロジェクト向けセクションを削除

### Version 1.1 (2025-12-21)

- 初期構造の確立

---

**Last Updated**: 2025-12-22
**Version**: 1.5
