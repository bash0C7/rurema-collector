# CLAUDE.md — rurema

## 概要
rurema/doctree の RD ファイルを BitClust でパースして収集する Collector gem。

## Collector インターフェース
- `collect(since: nil)` → `[{content:, source:}]`（since は無視）
- source 値: `rurema/doctree:ruby3.3/{lib}`, `rurema/doctree:ruby3.3/{lib}#{class}`
- DoctreeManager と RDParser を DI で差し替え可能（テスト用）

## 依存
- bitclust-core（github: rurema/bitclust）
