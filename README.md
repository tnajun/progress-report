# progress-report

Claude Code（デスクトップアプリ）の直近のセッションを読んで、**プロジェクトごとの進捗**と**途中で止まったまま忘れられていそうな作業**を、毎朝1枚の報告にまとめる Skill です。

- セッションの「できました」をうのみにせず、git・ファイル・本番 URL の実物で確かめてから書く
- 「GO 待ちのまま」「未コミットのまま」「下書きのまま」の作業を、**放っておくと困る順**に並べる
- セッション名はクリックでそのセッションに飛べるリンクになる
- 本人の返事待ちは、Claude の質問をそのまま1行で引用する
- **読むだけ**。送信・投稿・push・コミットは一切しない

## 入れ方

```
git clone https://github.com/tnajun/progress-report "$env:USERPROFILE\.claude\skills\progress-report"
```

`SKILL.md` の「0. 設定」を参考に、同じフォルダに `config.md` を置いて、自分のプロジェクト名・リポジトリ・本番 URL を書きます（なくても動きます）。

## 使い方

会話で「進捗報告して」と言うか、毎朝のルーティン（スケジュールタスク）に次の1行を入れます。

```
progress-report スキルで、今日の進捗報告を書いて。
```

判断待ちが出たときに通知したい場合は [routine-notify](https://github.com/tnajun/routine-notify) と組み合わせてください。

## 解説記事

[posii.net のコラム](https://posii.net/claude-code-progress-report/)

## License

MIT
