# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.4.0] - 2026-01-07

### Added
- **LLM最適化版テンプレート**: 4つのLLM向けに最適化されたプロンプトを追加
  - `templates/gpt/` - GPT-4o/5向け（41テンプレート）
    - 英語System Prompt見出し
    - IMPORTANT REMINDERS セクション
    - 推奨パラメータ設定（Temperature, Top-p等）
  - `templates/claude/` - Claude 4.x向け（41テンプレート）
    - XMLタグ構造化（`<system>`, `<role>`, `<knowledge>`, `<style>`, `<rules>`, `<workflow>`, `<constraints>`）
    - Claude Projects活用ガイド
    - Extended Thinking活用場面の提案
  - `templates/copilot/` - Microsoft Copilot向け（41テンプレート）
    - Role and Purpose見出し形式
    - M365 Integration Tips（Teams, SharePoint, Forms, Excel等）
    - KEY REMINDERS セクション
  - `templates/gemini/` - Gemini Pro向け（41テンプレート）
    - 太字見出し形式（**Role Definition**等）
    - Critical Rules セクション
    - Google Workspace Integration（Meet, Classroom, Drive等）

### Changed
- README.mdにLLM最適化版の説明を追加
- プロジェクト構造の図を更新

### Technical Details
- 合計164ファイルを新規作成（41テンプレート × 4 LLM）
- 各LLMの特性に基づく最適化パターンを適用（References/chapter10-ai-model-adaptation.md準拠）

---

## [1.3.0] - 2025-12-22

### Added
- コンパクト版テンプレート（`templates/compact/`）41種類を追加
  - 8,000文字以内に圧縮
  - トークン制限のあるAIモデル向け

### Changed
- ディレクトリ構造を再編成
  - `templates/full/` - フル版（詳細版）
  - `templates/compact/` - コンパクト版

---

## [1.2.0] - 2025-12-22

### Added
- 高等教育系テンプレート9種類を追加
  - 大学教員（university-faculty）
  - 研究指導者（research-supervisor）
  - FD担当者（faculty-developer）
  - キャリア支援（university-career-support）
  - 留学生支援（international-student-support）
  - 学生相談（university-student-counselor）
  - 学部長・学科長（academic-department-head）
  - 産学連携コーディネーター（industry-academia-coordinator）
  - 入試広報担当（admissions-officer）

### Changed
- 全41テンプレートに拡充

---

## [1.1.0] - 2025-12-21

### Added
- 全32テンプレートに回答品質強化セクションを追加
  - 思考チェーン（Chain of Thought）
  - 出力品質チェックリスト
  - エラー回復プロンプト
  - 回答の深さ調整ガイド
- AIモデル別適用ガイドを追加
  - Microsoft 365 Copilot対応
  - ChatGPT対応
  - Claude対応
  - Gemini対応

---

## [1.0.0] - 2025-12-20

### Added
- 初回リリース
- 32種類のInteractive Agentic Promptテンプレート
  - 学校現場系テンプレート
  - 教育行政系テンプレート
- 5フェーズアーキテクチャ
  - Phase 1: Discovery（発見）
  - Phase 2: Context Gathering（文脈収集）
  - Phase 3: SKILL Selection（理論選択）
  - Phase 4: Meta-Prompt Generation（メタプロンプト生成）
  - Phase 5: Response Generation（回答生成）
- ドキュメント
  - Interactive Agentic Prompt完全ガイド
  - IAP作成マニフェスト
