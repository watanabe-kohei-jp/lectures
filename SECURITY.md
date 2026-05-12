# Security Policy

このリポジトリは教育用 HTML スライド集です。ソフトウェア製品のような脆弱性は通常発生しませんが、以下のケースで報告経路を用意しています。

## 報告対象

| 種類 | 例 |
|---|---|
| **教材内容の重大な誤り** | 安全上問題のある手順、明らかな事実誤認、誘導されると損害を生む記述 |
| **秘密情報の混入疑い** | リポジトリの過去 commit に API キー・トークン・個人情報が残っている疑い |
| **悪意ある外部リンク** | 教材内のリンクが乗っ取られて悪意あるサイトに飛ぶ等 |
| **`prompt-injection-check.yml` の検知漏れ** | hidden な AI 命令が main に紛れ込んでいる |
| **HTML/JS の XSS 系** | 受講者の入力が `lecture.html` 内で危険に評価される等（実際にはほぼ発生しないはず）|

## 報告経路

### 推奨: GitHub Security Advisories（非公開で連絡）

[Security Advisories の新規作成ページ](https://github.com/watanabe-kohei-jp/lectures/security/advisories/new)から **private に** 連絡してください。発見者と作者の間だけで議論できます。

### 通常の誤りや教材改善は Issue / Discussion へ

「これ間違ってない？」というレベルの問い合わせは、通常の [Issue](https://github.com/watanabe-kohei-jp/lectures/issues) または [Discussion](https://github.com/watanabe-kohei-jp/lectures/discussions) で構いません。Security Advisories は **公開すると受講者に害が及ぶ可能性がある場合に限定** してください。

## 対応の目安

- 受領後 **7 日以内に一次返信**
- 重大度に応じて修正 PR を作成 → merge
- 修正後、報告者を希望すれば Acknowledgements として CREDITS.md に追記

個人で運営している教材リポなので SLA は保証しません。緊急性が高い場合はその旨明記してください。

## 報告者の保護

- 善意で報告いただいた方を法的に追及することはありません
- 報告内容が「事実と異なる」場合も、議論のうえ穏当に終わらせます
