# Lecture 01 — AI ネイティブ世代の Git / GitHub 入門

大学の同期・後輩 5 名向け、90 分対面のハンズオン講義。第 1 回。

## 構成

```
01-git-github/
├── handson/                    ← ハンズオン用の作業ディレクトリ（ローカル限定、.gitignore 済み）
│   ├── Asan/
│   └── Bsan/
├── plan.md                     ← Claude Plan モードで書いた当初の追加プラン
├── source-structure.md         ← スライド構成（旧 39 枚 → 新 36 枚への組み直し設計）
└── README.md                   ← このファイル
```

## 講義の方針

| 軸 | 内容 |
|---|---|
| 聴衆 | 大学の同期・後輩 5 名（CLI 未経験前提） |
| 時間 | 90 分・対面 |
| ゴール | ① Git/GitHub の必要性を体感 ② 実際に触る ③ AI 時代の使い方を知る |
| トーン | 静か・知的（OpenAI / Anthropic 風）、白基調＋テラコッタ |
| アナロジー | Word vs Google Drive のみ（ドラクエは没にした） |

## ハンズオンの設計

受講者は基本操作（clone / 自分のファイル commit & push）まで。
コンフリクトの実演は発表者が `handson/Asan` と `handson/Bsan` を使って前で見せる。

実演の流れ（既に動作確認済み）：
1. `Asan` で README 編集 → commit → push（成功）
2. `Bsan` で同じ行を別の内容で編集 → commit → push（**rejected**）
3. `Bsan` で pull → コンフリクト発生（マーカー出現）
4. 両方の変更を残す形で解決 → commit → push
5. `git log --oneline --graph` で Y 字のマージグラフを見せる

## シリーズ計画（暫定）

| 回 | テーマ |
|---|---|
| 01 | Git / GitHub 入門（今回） |
| 02 | ブランチ / Pull Request / AI に任せる |
| 03 | Claude Code 実践（コード書き） |
