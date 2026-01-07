# プロンプト評価レポート

> 📅 評価日: 2026-01-07
> 🤖 評価者: GitHub Copilot (Claude Opus 4.5)

## 評価概要

| 項目 | 説明 |
|------|------|
| 評価対象 | 全41テンプレート × 3 LLM（GPT, Claude, Copilot） |
| 評価基準 | 構造整合性、LLM固有フォーマット準拠、サイズ |

---

## 1. サイズ評価サマリ

| LLM | テンプレート数 | 合計サイズ | 8000バイト超過 |
|-----|--------------|-----------|---------------|
| GPT | 41 | 254,945 bytes | 0件 ✅ |
| Claude | 41 | 276,449 bytes | 3件 ⚠️ |
| Copilot | 41 | 278,082 bytes | 2件 ⚠️ |

### 8000バイト超過ファイル

**Claude版:**
| ファイル | サイズ |
|---------|-------|
| club-activity-advisor | 8,124 bytes |
| career-counselor | 8,134 bytes |
| academic-department-head | 8,265 bytes |

**Copilot版:**
| ファイル | サイズ |
|---------|-------|
| parent-relations | 8,020 bytes |
| academic-department-head | 8,194 bytes |

---

## 2. LLM固有フォーマット準拠評価

### GPT-4o/GPT-5 版 ✅ 全41件準拠

| チェック項目 | 結果 |
|-------------|------|
| `System Prompt` セクション | 41/41 ✅ |
| `IMPORTANT REMINDERS` セクション | 41/41 ✅ |

**判定: 100% 準拠** ⭐⭐⭐⭐⭐

---

### Claude 4.x 版 ⚠️ 14件で `<constraints>` タグ欠如

| チェック項目 | 結果 |
|-------------|------|
| `<system>` タグ | 41/41 ✅ |
| `<role>` タグ | 41/41 ✅ |
| `<knowledge>` タグ | 41/41 ✅ |
| `<constraints>` タグ | 27/41 ⚠️ |

**欠如ファイル（14件）:**
1. curriculum-coordinator
2. education-center
3. faculty-developer
4. grade-leader
5. ict-education-coordinator
6. school-supervisor
7. school-transition-coordinator
8. social-education-coordinator
9. special-activities-coordinator
10. special-needs-supervisor
11. student-guidance
12. student-guidance-supervisor
13. superintendent
14. teacher-mentor

**判定: 66% 準拠** ⭐⭐⭐

---

### Microsoft Copilot 版 ⚠️ 3件でセクション欠如

| チェック項目 | 結果 |
|-------------|------|
| `# Role and Purpose` | 41/41 ✅ |
| `## Your Expertise` | 38/41 ⚠️ |
| `## Response Guidelines` | 38/41 ⚠️ |

**欠如ファイル（3件）:**
1. university-career-support
2. university-faculty
3. university-student-counselor

**判定: 93% 準拠** ⭐⭐⭐⭐

---

## 3. 総合評価

| LLM | サイズ | フォーマット | 総合判定 |
|-----|--------|------------|---------|
| **GPT** | ✅ 全件OK | ✅ 100% | ⭐⭐⭐⭐⭐ 優秀 |
| **Claude** | ⚠️ 3件超過 | ⚠️ 66% | ⭐⭐⭐ 要改善 |
| **Copilot** | ⚠️ 2件超過 | ⚠️ 93% | ⭐⭐⭐⭐ 良好 |

---

## 4. 改善アクションリスト

### 優先度: 高
- [ ] Claude版 14件に `<constraints>` タグを追加
- [ ] Copilot版 3件（university系）のセクション構造を修正

### 優先度: 中
- [ ] Claude版 3件のサイズ削減（8000バイト以下へ）
- [ ] Copilot版 2件のサイズ削減

---

## 評価メタデータ

```yaml
evaluation:
  date: 2026-01-07
  evaluator: GitHub Copilot (Claude Opus 4.5)
  method: Automated structural analysis + Manual review
  scope:
    llm_versions: [GPT, Claude, Copilot]
    templates_per_llm: 41
    total_files: 123
  results:
    gpt: PASS (100%)
    claude: NEEDS_IMPROVEMENT (66%)
    copilot: GOOD (93%)
```
