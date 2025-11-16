# Claude Code 開発効率化サブエージェント集

Claude Codeでの開発ワークフローを劇的に効率化する専門サブエージェントコレクション

## 🎯 プロジェクト概要

このプロジェクトは、Claude Codeを使った開発を高速化・高品質化するための専門サブエージェント群です。各エージェントは単一責任原則に基づいて設計され、特定の開発タスクに特化した支援を提供します。

### 🚀 効果

- **開発速度向上**: テスト作成、デバッグ、ドキュメント生成の自動化
- **コード品質向上**: セキュリティ監査、リファクタリング提案、コードレビュー
- **チーム標準化**: 一貫したコミットメッセージ、API設計パターン
- **専門特化支援**: フロントエンド/バックエンド特化、パフォーマンス最適化、データベース設計

## 目次

- [サブエージェント一覧](#サブエージェント一覧)
  - [Phase 1: 必須・高インパクト エージェント](#phase-1-必須高インパクト-エージェント)
  - [Phase 2: セキュリティ・アーキテクチャ エージェント](#phase-2-セキュリティアーキテクチャ-エージェント)
  - [Phase 3: 専門特化エージェント](#phase-3-専門特化エージェント)
- [セットアップ・使用方法](#セットアップ使用方法)
- [エージェント選択ガイドライン](#エージェント選択ガイドライン)
- [使用例とベストプラクティス](#使用例とベストプラクティス)
- [統合手順](#統合手順)
- [効果測定指標](#効果測定指標)

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

#### 🎨 code-formatter (Haiku)

**専門分野**: コード書式設定

- 多言語対応自動フォーマット
- markdownlint準拠
- プロジェクト固有スタイル適用
- バッチ処理・CI/CD統合

**使用タイミング**: コミット前、コードレビュー前、プロジェクト標準化時

### Phase 3: 専門特化エージェント

#### 🌐 frontend-specialist (Sonnet)

**専門分野**: フロントエンド開発支援

**主要機能**:

- React/Vue/Angular最適化パターン
- モダンCSS・スタイリングソリューション
- パフォーマンス最適化（Core Web Vitals）
- バンドル最適化・コード分割戦略
- アクセシビリティベストプラクティス

**使用タイミング**:

- フロントエンド設計・アーキテクチャ決定時
- UIコンポーネント開発・最適化時
- パフォーマンス問題解決時

#### 🔧 backend-specialist (Sonnet)

**専門分野**: バックエンド開発支援

**主要機能**:

- Node.js/Python/Java/Go サーバー開発
- マイクロサービス・API設計パターン
- データベース統合・ORM最適化
- 分散システム・スケーラビリティ対策
- セキュリティ・認証実装

**使用タイミング**:

- サーバーアーキテクチャ設計時
- API開発・最適化時
- スケーラビリティ課題解決時

#### ⚡ performance-analyzer (Sonnet)

**専門分野**: パフォーマンス分析・最適化

**主要機能**:

- フロントエンド・バックエンドパフォーマンス分析
- Core Web Vitals最適化
- データベースクエリ最適化
- メモリ管理・キャッシュ戦略
- モバイル・ネットワーク最適化

**使用タイミング**:

- パフォーマンス問題の根本原因調査時
- 最適化戦略立案時
- 定期的なパフォーマンス監査時

#### 🗄️ database-designer (Sonnet)

**専門分野**: データベース設計・最適化

**主要機能**:

- リレーショナル・NoSQLデータベース設計
- スキーマ設計・正規化戦略
- インデックス最適化・クエリ改善
- データマイグレーション戦略
- CQRS・イベントソーシングパターン

**使用タイミング**:

- データベース設計・リアーキテクチャ時
- クエリパフォーマンス問題解決時
- データモデリング・マイグレーション計画時

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

# Phase 1: 必須エージェント
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/test-generator.md -O .claude/agents/test-generator.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/bug-analyzer.md -O .claude/agents/bug-analyzer.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/documentation-generator.md -O .claude/agents/documentation-generator.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/commit-message-generator.md -O .claude/agents/commit-message-generator.md

# Phase 2: セキュリティ・アーキテクチャ
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/security-scanner.md -O .claude/agents/security-scanner.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/api-designer.md -O .claude/agents/api-designer.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/refactoring-advisor.md -O .claude/agents/refactoring-advisor.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/code-reviewer.md -O .claude/agents/code-reviewer.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/code-formatter.md -O .claude/agents/code-formatter.md

# Phase 3: 専門特化エージェント
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/frontend-specialist.md -O .claude/agents/frontend-specialist.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/backend-specialist.md -O .claude/agents/backend-specialist.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/performance-analyzer.md -O .claude/agents/performance-analyzer.md
wget https://raw.githubusercontent.com/glkt3912/claude-code-subagents/main/.claude/agents/database-designer.md -O .claude/agents/database-designer.md
```

### エージェント配置確認

```bash
ls -la .claude/agents/
# 以下のファイルが配置されていることを確認

# Phase 1: 必須・高インパクト (4つ)
# - test-generator.md
# - bug-analyzer.md
# - documentation-generator.md
# - commit-message-generator.md

# Phase 2: セキュリティ・アーキテクチャ (5つ)
# - security-scanner.md
# - api-designer.md
# - refactoring-advisor.md
# - code-reviewer.md
# - code-formatter.md

# Phase 3: 専門特化 (4つ)
# - frontend-specialist.md
# - backend-specialist.md
# - performance-analyzer.md
# - database-designer.md

# 合計: 13のエージェント
```

### Claude Codeでの使用

1. **Claude Codeを起動**
2. **エージェント確認**: `/agents` コマンドで利用可能なエージェント一覧を確認
3. **エージェント選択**: `@エージェント名` でエージェントを切り替え
4. **タスク実行**: 目的に応じたエージェントで作業を実行

### エージェント選択ガイドライン

| 開発フェーズ | 推奨エージェント | 目的 |
|-------------|----------------|------|
| **プロジェクト設計** | api-designer, database-designer | API設計、データベース設計 |
| **実装・開発** | frontend-specialist, backend-specialist | 専門領域特化開発 |
| **品質管理** | test-generator, code-formatter | テスト作成、コード整形 |
| **デバッグ・分析** | bug-analyzer, performance-analyzer | 問題調査、パフォーマンス分析 |
| **レビュー・監査** | code-reviewer, security-scanner | コードレビュー、セキュリティ監査 |
| **最適化・改善** | refactoring-advisor, performance-analyzer | リファクタリング、性能改善 |
| **ドキュメント** | documentation-generator | 文書作成・更新 |
| **コミット・管理** | commit-message-generator | Git履歴管理 |

## 📋 使用例とベストプラクティス

### 🔄 段階的活用アプローチ

#### ステップ1: 基本エージェントから開始

```bash
# 最初に導入すべきエージェント（Phase 1）
@test-generator         # テスト自動生成
@documentation-generator # ドキュメント作成
@commit-message-generator # コミットメッセージ
```

#### ステップ2: 品質向上エージェント追加

```bash
# コード品質向上のため（Phase 2）
@code-reviewer         # コードレビュー
@security-scanner      # セキュリティ監査
@code-formatter       # コード整形
```

#### ステップ3: 専門特化エージェント活用

```bash
# プロジェクトの特性に応じて（Phase 3）
@frontend-specialist   # フロントエンド特化
@backend-specialist    # バックエンド特化
@performance-analyzer  # パフォーマンス分析
@database-designer     # データベース設計
```

### 🎯 エージェント組み合わせパターン

#### Web アプリケーション開発

```text
設計フェーズ:
1. @api-designer → API設計
2. @database-designer → データモデル設計
3. @documentation-generator → API仕様書作成

実装フェーズ:
1. @frontend-specialist → UI/UXコンポーネント開発
2. @backend-specialist → サーバーサイド実装
3. @test-generator → テストケース作成

品質保証フェーズ:
1. @code-formatter → コード整形
2. @code-reviewer → コードレビュー
3. @security-scanner → セキュリティ監査
4. @performance-analyzer → パフォーマンステスト
```

#### モバイルアプリ開発

```text
1. @frontend-specialist → UI最適化（React Native/Flutter）
2. @performance-analyzer → メモリ・バッテリー最適化
3. @security-scanner → モバイル固有脆弱性チェック
4. @test-generator → デバイス別テストケース
```

### 🎨 各エージェント活用例

#### Phase 1: 基本エージェント

**test-generator の活用例**:

```text
# 新機能のテスト生成
"この calculateTotalPrice 関数の包括的なテストスイートを作成してください。エッジケースも含めて"

# 既存コードのカバレッジ向上
"このユーザー認証モジュールで未テストのパスを特定し、必要なテストケースを追加してください"

# モックオブジェクト生成
"この API クライアントクラスの Jest テストを作成し、適切なモック設定も含めてください"
```

**documentation-generator の活用例**:

```text
# README作成
"このプロジェクトの README.md を作成してください。セットアップ手順と使用例も含めて"

# API ドキュメント生成
"この Express.js API の OpenAPI 3.0 仕様書を生成してください"

# コードコメント追加
"この関数に JSDoc コメントを追加してください。パラメータと戻り値の説明も含めて"
```

#### Phase 2: 品質向上エージェント

**security-scanner の活用例**:

```text
# セキュリティ監査
"この認証システムを OWASP Top 10 の観点から監査してください"

# 依存関係チェック
"package.json の依存関係で既知の脆弱性を確認し、対策案を提示してください"

# コード脆弱性分析
"この SQL クエリ処理にインジェクション脆弱性がないか検査してください"
```

**code-reviewer の活用例**:

```text
# コードレビュー実施
"この Pull Request の変更内容をレビューし、改善点を指摘してください"

# ベストプラクティス確認
"この React コンポーネントがベストプラクティスに従っているかチェックしてください"

# アーキテクチャ評価
"このマイクロサービスの設計について、保守性の観点からフィードバックをください"
```

#### Phase 3: 専門特化エージェント

**frontend-specialist の活用例**:

```text
# React パフォーマンス最適化
"この React コンポーネントのレンダリング性能を向上させる方法を提案してください"

# CSS 最適化
"このスタイルシートを CSS-in-JS に移行し、パフォーマンスを改善してください"

# アクセシビリティ改善
"このフォームコンポーネントを WCAG 2.1 に準拠させるための修正案を提示してください"
```

**backend-specialist の活用例**:

```text
# API 設計改善
"この REST API を GraphQL に移行する際の設計案を提案してください"

# データベース最適化
"この ORM クエリのN+1問題を解決し、パフォーマンスを改善してください"

# マイクロサービス設計
"このモノリスをマイクロサービスに分割する戦略を立ててください"
```

**performance-analyzer の活用例**:

```text
# ページ速度最適化
"この Web ページの Lighthouse スコアを改善する具体的な方法を教えてください"

# データベース性能改善
"この遅いクエリを分析し、インデックス戦略を提案してください"

# メモリ使用量最適化
"この Node.js アプリケーションのメモリリークを特定し、修正してください"
```

**database-designer の活用例**:

```text
# スキーマ設計
"この e-commerce システム用の正規化されたデータベーススキーマを設計してください"

# クエリ最適化
"この複雑な JOIN クエリを最適化し、実行計画も改善してください"

# データ移行計画
"MySQL から PostgreSQL へのマイグレーション計画を立ててください"
```

### 🔧 統合手順

#### CI/CD パイプライン統合

```yaml
# .github/workflows/claude-agents.yml
name: Claude Agents Quality Check

on: [push, pull_request]

jobs:
  quality-check:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v3
    
    # コードフォーマット確認
    - name: Code Format Check
      run: |
        # @code-formatter による整形済みかチェック
        
    # セキュリティスキャン
    - name: Security Scan
      run: |
        # @security-scanner による脆弱性チェック
        
    # テストカバレッジ
    - name: Test Coverage
      run: |
        # @test-generator で生成されたテストの実行
```

#### pre-commit hook 設定

```bash
# .git/hooks/pre-commit
#!/bin/sh

# コード整形
echo "Running code formatter..."
claude-code @code-formatter "プロジェクト全体のコードを整形してください"

# コミットメッセージ生成
echo "Generating commit message..."
COMMIT_MSG=$(claude-code @commit-message-generator "git diff --cached の内容からコミットメッセージを生成してください")

echo "$COMMIT_MSG" > .git/COMMIT_EDITMSG
```

### 👥 チーム開発ワークフロー

#### エージェント役割分担例

```text
設計担当者:
- @api-designer: API仕様策定
- @database-designer: データモデル設計
- @documentation-generator: 設計書作成

フロントエンド開発者:
- @frontend-specialist: UI/UX実装
- @test-generator: フロントエンドテスト
- @performance-analyzer: 描画性能最適化

バックエンド開発者:
- @backend-specialist: サーバーサイド実装
- @database-designer: クエリ最適化
- @security-scanner: API セキュリティ

DevOps エンジニア:
- @performance-analyzer: インフラ監視
- @security-scanner: システム監査
- @code-formatter: CI/CD 統合

全員共通:
- @commit-message-generator: Git 履歴管理
- @code-reviewer: プルリクエストレビュー
```

## 📈 効果測定指標

### 開発効率向上

| メトリクス | 目標改善率 | 測定方法 |
|-----------|-----------|---------|
| **テスト作成時間** | 70%短縮 | @test-generator使用前後の時間計測 |
| **ドキュメント作成時間** | 80%短縮 | @documentation-generator使用前後 |
| **デバッグ時間** | 50%短縮 | @bug-analyzer使用による問題解決時間 |
| **コードレビュー時間** | 40%短縮 | @code-reviewer事前チェック効果 |
| **リファクタリング時間** | 60%短縮 | @refactoring-advisor提案の活用効果 |

### コード品質改善

| メトリクス | 目標改善 | 専門エージェント |
|-----------|--------|----------------|
| **セキュリティ脆弱性** | 90%削減 | @security-scanner |
| **パフォーマンス問題** | 80%削減 | @performance-analyzer |
| **コード規約違反** | 95%削減 | @code-formatter |
| **バグ発生率** | 60%削減 | @test-generator + @bug-analyzer |
| **技術的負債** | 70%削減 | @refactoring-advisor |

### チーム生産性向上

| メトリクス | 目標改善 | 対象エージェント |
|-----------|--------|----------------|
| **新規メンバー教育時間** | 50%短縮 | @documentation-generator |
| **コミット履歴品質** | 100%向上 | @commit-message-generator |
| **コードレビュー品質** | 80%向上 | @code-reviewer |
| **知識共有効率** | 60%向上 | 専門特化エージェント群 |

### 専門領域効果測定

#### フロントエンド開発 (@frontend-specialist)

- **Core Web Vitals スコア**: 平均20%向上
- **バンドルサイズ**: 30%削減
- **開発速度**: React/Vue/Angularコンポーネント作成時間50%短縮

#### バックエンド開発 (@backend-specialist)

- **API応答時間**: 40%改善
- **データベースクエリ効率**: 60%向上
- **スケーラビリティ**: 同時接続数2倍対応

#### パフォーマンス (@performance-analyzer)

- **ページ読み込み速度**: 50%改善
- **メモリ使用量**: 30%削減
- **レスポンス時間**: 平均40%短縮

#### データベース設計 (@database-designer)

- **クエリ実行時間**: 70%改善
- **データ整合性エラー**: 90%削減
- **スキーマ最適化**: インデックス効率80%向上

## 🛠️ メンテナンス・発展計画

### 定期見直しサイクル

#### 🔄 月次レビュー

**実施内容**:

- エージェント使用頻度・効果分析
- 新機能リクエスト収集
- パフォーマンス指標確認
- チームフィードバック収集

**チェックポイント**:

```text
✅ 各エージェントの利用状況確認
✅ 開発効率指標のトラッキング
✅ 新しい開発パターンへの対応検討
✅ エージェント組み合わせ最適化
```

#### 📊 四半期アップデート

**実施内容**:

- プロジェクト変化に応じた調整
- 新技術トレンドへの対応
- エージェント機能拡張
- 統合ツールアップデート

**主要タスク**:

```text
🔧 プロジェクト固有設定の見直し
🔧 新フレームワーク対応追加
🔧 CI/CD統合の最適化
🔧 チーム教育プログラム更新
```

#### 🚀 半期リニューアル

**実施内容**:

- 業界ベストプラクティス反映
- 新エージェント追加検討
- 大幅な機能改善実装
- ROI評価と戦略見直し

### 🌟 今後の発展予定

#### Phase 4: 高度統合エージェント（計画中）

```text
🤖 devops-assistant (Sonnet)
- CI/CD パイプライン最適化
- インフラ自動化・監視
- デプロイメント戦略提案
- コンテナ・K8s最適化

📊 project-manager (Sonnet) 
- タスク分解・見積もり自動化
- プロジェクト進捗追跡
- リスク分析・対策提案
- リソース配分最適化

🧠 ai-architect (Sonnet)
- AI/ML システム設計
- データパイプライン構築
- モデル最適化戦略
- MLOps ベストプラクティス

🔒 compliance-auditor (Sonnet)
- 法規制対応チェック
- GDPR/CCPA準拠確認
- 業界標準適合性監査
- ドキュメント自動生成
```

#### Phase 5: エコシステム統合（長期計画）

```text
🌐 外部ツール統合
- GitHub Actions深度統合
- Slack/Teams通知システム
- Jira/Asanaタスク連携
- Figma/デザインツール連携

📱 モバイル専用エージェント
- iOS/Android最適化
- App Store最適化
- モバイルセキュリティ特化
- デバイス固有問題解決

☁️ クラウド特化エージェント  
- AWS/Azure/GCP最適化
- サーバーレス設計支援
- コスト最適化提案
- マルチクラウド戦略
```

### 🎯 継続改善フレームワーク

#### PDCA サイクル

```text
📋 Plan (計画)
- エージェント機能拡張計画
- チーム教育スケジュール
- 新技術対応ロードマップ

⚡ Do (実行)  
- エージェント定期アップデート
- チーム内ベストプラクティス共有
- 新機能テスト・導入

📊 Check (評価)
- KPI指標測定・分析
- ユーザーフィードバック収集
- ROI評価・効果検証

🔄 Act (改善)
- 問題点の修正実装
- プロセス最適化
- 次期計画への反映
```

### 🤝 コミュニティ貢献

#### オープンソース化計画

```text
📂 コミュニティ版リリース
- 基本エージェント群の公開
- カスタマイズガイド提供
- ベストプラクティス集公開

🤝 コミュニティ運営
- Issues/PRレビュー対応
- 月次コミュニティ会議開催
- ユーザー事例収集・共有

📚 教育リソース
- オンライン学習コース作成
- 実践ワークショップ開催
- 認定プログラム検討
```

## 🤝 コントリビューション

### 改善提案の方法

#### Issue作成ガイドライン

```text
🐛 バグ報告
- エージェント名と問題の詳細
- 再現手順と期待される動作
- 使用環境の情報

💡 機能要求
- 新機能の概要と必要性
- 具体的な使用場面
- 実装案があれば記載

📝 ドキュメント改善
- 不明確な部分の指摘
- 使用例の追加提案
- 翻訳・多言語対応
```

#### Pull Request ガイドライン

```text
✅ エージェント定義の改善
- 既存機能の拡張・最適化
- 新しいユースケースの追加
- パフォーマンス改善

✅ ドキュメント更新
- README.md の改善
- 使用例の追加
- ベストプラクティス共有

✅ テンプレート提供
- プロジェクト固有設定例
- 業界別カスタマイズ例
- 統合手順の詳細化
```

### カスタムエージェント開発

#### 開発ガイド

```text
📋 企画・設計
1. エージェントの目的・スコープ定義
2. 既存エージェントとの差別化確認
3. ターゲットユーザー・使用場面特定

🔧 実装
1. 既存エージェントテンプレート活用
2. チーム固有ニーズの反映
3. 単一責任原則の遵守

✅ テスト・検証  
1. 実プロジェクトでの動作確認
2. パフォーマンス・品質評価
3. チーム内フィードバック収集

📤 共有・提供
1. ドキュメント整備
2. コミュニティへの貢献
3. 継続的な改善・アップデート
```
