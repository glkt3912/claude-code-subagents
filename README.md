# Claude Code 開発効率化サブエージェント集

Claude Codeでの開発ワークフローを劇的に効率化する専門サブエージェントコレクション

## 🎯 プロジェクト概要

このプロジェクトは、Claude Codeを使った開発を高速化・高品質化するための専門サブエージェント群です。各エージェントは単一責任原則に基づいて設計され、特定の開発タスクに特化した支援を提供します。

### 🚀 効果

- **開発速度向上**: テスト作成、デバッグ、ドキュメント生成の自動化
- **コード品質向上**: セキュリティ監査、リファクタリング提案、コードレビュー
- **チーム標準化**: 一貫したコミットメッセージ、API設計パターン

## 📦 サブエージェント一覧

### Phase 1: 必須・高インパクト エージェント

#### 🧪 test-generator (Sonnet)

**専門分野**: テスト自動生成

- ユニットテスト・統合テストの作成
- モック・テストデータ生成
- エッジケース検出とカバレッジ向上
- 各種テストフレームワーク対応

**使用タイミング**: 新機能実装後、バグ修正時、テストカバレッジ向上時

#### 🔍 bug-analyzer (Sonnet)

**専門分野**: バグ解析・デバッグ支援

- エラーメッセージ・スタックトレース解析
- 根本原因特定と修正提案
- パフォーマンス問題検出
- デバッグ戦略立案

**使用タイミング**: エラー発生時、予期しない動作時、パフォーマンス問題時

#### 📚 documentation-generator (Sonnet)

**専門分野**: ドキュメント生成

- README、API仕様書、コードコメント
- OpenAPI/Swagger対応
- 技術文書・使用例の自動生成
- オンボーディング資料作成

**使用タイミング**: 新プロジェクト開始時、API作成時、ドキュメント更新時

#### 💬 commit-message-generator (Haiku)

**専門分野**: コミットメッセージ作成

- Conventional Commits準拠
- 変更内容の適切な分類とスコープ検出
- git履歴の整理・検索性向上
- チーム標準の統一

**使用タイミング**: 毎回のgitコミット前

### Phase 2: セキュリティ・アーキテクチャ エージェント

#### 🛡️ security-scanner (Sonnet)

**専門分野**: セキュリティ監査

- OWASP Top 10脆弱性検出
- 依存関係のセキュリティ分析
- セキュアコーディング評価
- リスクアセスメント

**使用タイミング**: セキュリティレビュー時、本番デプロイ前、定期監査

#### 🏗️ api-designer (Sonnet)

**専門分野**: API設計支援

- REST/GraphQL設計パターン
- エンドポイント命名規則・バージョニング
- OpenAPI仕様書生成
- 開発者体験の最適化

**使用タイミング**: API設計時、既存API見直し時、仕様書作成時

#### ♻️ refactoring-advisor (Sonnet)

**専門分野**: リファクタリング顧問

- コードスメル検出
- パフォーマンス最適化提案
- 段階的改善計画
- レガシーコード現代化

**使用タイミング**: コード品質向上時、技術的負債解消時、保守性改善時

#### ✅ code-reviewer (Sonnet)

**専門分野**: コードレビュー

- 品質・ベストプラクティス評価
- セキュリティ・パフォーマンス観点
- 建設的フィードバック提供
- 学習・継続改善支援

**使用タイミング**: コード実装完了時、機能追加時、バグ修正後

## 🚀 セットアップ・使用方法

### 新規プロジェクトでの導入

#### 方法1: Git Clone（推奨）

```bash
# 既存プロジェクトのディレクトリで実行
git clone https://github.com/glkt3912/claude-code-subagents.git temp-agents
cp -r temp-agents/.claude ./
rm -rf temp-agents

# または一行で
curl -L https://github.com/glkt3912/claude-code-subagents/archive/main.zip | unzip -j - "claude-code-subagents-main/.claude/agents/*" -d .claude/agents/
```

#### 方法2: Git Submodule

```bash
# サブモジュールとして追加（更新も容易）
git submodule add https://github.com/glkt3912/claude-code-subagents.git .claude/subagents
ln -s .claude/subagents/.claude/agents .claude/agents

# 更新時
git submodule update --remote
```

#### 方法3: 選択的導入

```bash
# 特定のエージェントのみ導入
mkdir -p .claude/agents
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/test-generator.md -O .claude/agents/test-generator.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/security-scanner.md -O .claude/agents/security-scanner.md
```

### エージェント配置確認

```bash
ls -la .claude/agents/
# 以下のファイルが配置されていることを確認
# - api-designer.md
# - bug-analyzer.md
# - code-reviewer.md
# - commit-message-generator.md
# - documentation-generator.md
# - refactoring-advisor.md
# - security-scanner.md
# - test-generator.md
```

### 2. Claude Codeでの使用

1. Claude Codeを起動
2. `/agents` コマンドでエージェント一覧確認
3. 目的に応じたエージェントを選択して使用

### 3. エージェント選択ガイドライン

| 開発フェーズ | 推奨エージェント | 目的 |
|-------------|----------------|------|
| 設計・計画 | api-designer | API設計、仕様策定 |
| 実装中 | test-generator, documentation-generator | テスト駆動開発、ドキュメント整備 |
| デバッグ | bug-analyzer | 問題解決、根本原因分析 |
| レビュー | code-reviewer, security-scanner | 品質保証、セキュリティ確保 |
| リファクタリング | refactoring-advisor | 技術的負債解消、保守性向上 |
| コミット | commit-message-generator | 一貫したgit履歴管理 |

## 📋 ベストプラクティス

### 🔄 段階的活用アプローチ

1. **導入**: まずは1つのエージェントから開始
2. **習熟**: 実際の開発で使いながらカスタマイズ
3. **展開**: チーム全体での活用拡大
4. **最適化**: プロジェクトに合わせた継続改善

### 🎯 単一責任の原則

- 各エージェントは特定の専門分野に集中
- 複数エージェントの組み合わせで包括的サポート
- 機能重複の排除と明確な責任境界

### 👥 チーム共有戦略

- `.claude/agents/` の git管理
- カスタマイズ履歴の文書化
- チーム内ベストプラクティス共有
- 定期的な効果測定と改善

### 🔧 カスタマイズのコツ

- プロジェクト固有の語彙・パターンを追加
- チームのコーディング規約を反映
- 使用頻度に応じたプロンプト調整
- フィードバックを基にした継続改善

## 🎨 各エージェント詳細

### test-generator の活用例

```bash
# 新しい関数のテストを生成
"この calculateTotalPrice 関数の包括的なテストスイートを作成してください"

# 既存テストのカバレッジ向上
"ユーザー認証モジュールで未テストのエッジケースを特定し、テストを追加してください"
```

### security-scanner の活用例

```bash
# セキュリティ監査実施
"このAPIエンドポイントをOWASP Top 10の観点でレビューしてください"

# 依存関係チェック
"package.jsonの依存関係で既知の脆弱性をチェックしてください"
```

### commit-message-generator の活用例

```bash
# ステージされた変更の分析
"git diff --cached の内容を分析して適切なコミットメッセージを生成してください"
```

## 🛠️ メンテナンス・発展計画

### 定期見直しサイクル

#### 月次レビュー

- 各エージェントの使用頻度分析
- 効果測定と改善点特定
- 新しい開発パターンへの対応

#### 四半期アップデート

- プロジェクト変化に合わせた調整
- 新技術・フレームワークへの対応
- チームフィードバックの反映

#### 半年リニューアル

- 業界トレンドに基づく機能追加
- パフォーマンス最適化
- 新エージェント追加検討

### 🌟 Phase 3 実装予定

#### 専門特化エージェント

- **frontend-specialist**: React/Vue/Angular最適化
- **backend-specialist**: サーバーサイド専門支援
- **performance-analyzer**: パフォーマンス分析・最適化
- **database-designer**: DB設計・最適化

#### ワークフロー統合エージェント

- **devops-assistant**: CI/CD、インフラ設計
- **project-manager**: タスク分解、見積もり支援

## 📈 効果測定指標

### 開発効率

- テスト作成時間の短縮
- バグ修正時間の削減
- ドキュメント作成の自動化率

### コード品質

- セキュリティ脆弱性の早期発見
- コードレビュー指摘事項の減少
- 技術的負債の継続的改善

### チーム生産性

- コミットメッセージの一貫性向上
- オンボーディング時間の短縮
- 知識共有の促進

## 🤝 コントリビューション

### 改善提案

1. Issue作成で改善要望を共有
2. Pull Requestでエージェント定義の改善
3. 使用事例・ベストプラクティスの共有

### カスタムエージェント開発

1. 既存エージェントをテンプレートとして活用
2. チーム固有のニーズに合わせたエージェント作成
3. コミュニティへのナレッジ共有
