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
| Claude | 41 | ~275,600 bytes | 0件 ✅ (修正済) |
| Copilot | 41 | ~277,700 bytes | 0件 ✅ (修正済) |

### サイズ超過修正完了

**Claude版（修正前→修正後）:**
| ファイル | 修正前 | 修正後 |
|---------|-------|-------|
| academic-department-head | 8,265 bytes | 7,971 bytes ✅ |
| career-counselor | 8,134 bytes | 7,878 bytes ✅ |
| club-activity-advisor | 8,124 bytes | 7,868 bytes ✅ |

**Copilot版（修正前→修正後）:**
| ファイル | 修正前 | 修正後 |
|---------|-------|-------|
| academic-department-head | 8,194 bytes | 8,000 bytes ✅ |
| parent-relations | 8,020 bytes | 7,813 bytes ✅ |

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
| **Claude** | ✅ 全件OK (修正済) | ✅ 100% (修正済) | ⭐⭐⭐⭐⭐ 優秀 |
| **Copilot** | ✅ 全件OK (修正済) | ✅ 100% (修正済) | ⭐⭐⭐⭐⭐ 優秀 |

---

## 4. 修正履歴

### 2026-01-07 修正適用済み

**Claude版（14件）** - `<constraints>` タグ追加完了:
- ✅ curriculum-coordinator, education-center, faculty-developer
- ✅ grade-leader, ict-education-coordinator, school-supervisor
- ✅ school-transition-coordinator, social-education-coordinator
- ✅ special-activities-coordinator, special-needs-supervisor
- ✅ student-guidance, student-guidance-supervisor
- ✅ superintendent, teacher-mentor

**Copilot版（3件）** - セクション構造修正完了:
- ✅ university-career-support: `## Your Expertise` / `## Response Guidelines` 追加
- ✅ university-faculty: `## Your Expertise` / `## Response Guidelines` 追加
- ✅ university-student-counselor: `## Your Expertise` / `## Response Guidelines` 追加

**サイズ超過修正（5件）** - 変更履歴セクション削除:
- ✅ Claude: academic-department-head (8,265 → 7,971 bytes)
- ✅ Claude: career-counselor (8,134 → 7,878 bytes)
- ✅ Claude: club-activity-advisor (8,124 → 7,868 bytes)
- ✅ Copilot: academic-department-head (8,194 → 8,000 bytes)
- ✅ Copilot: parent-relations (8,020 → 7,813 bytes)

---

## 5. 残課題

**すべての課題が解決されました** ✅

- ~~Claude版 3件のサイズ削減~~ → 完了
- ~~Copilot版 2件のサイズ削減~~ → 完了

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
    claude: PASS (100% - fixed)
    copilot: PASS (100% - fixed)
  fixes_applied:
    claude: 14 files (added <constraints> tags) + 3 files (size reduction)
    copilot: 3 files (added Your Expertise/Response Guidelines) + 2 files (size reduction)
```
