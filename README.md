# fizz-thinking-cue-detector

**Fizz** (AITuber system in [Almide](https://github.com/almide/almide)) — §3 brain 部品。

発話する文が思考モーションを出すべきか判定 (発話中のみ)。`should_play_thinking(fragment) -> Bool`。idle/応答待ちからは呼ばない。

責務は一行で、入力 → 出力が型で言い切れる単位 (openaituber `docs/almide-component-breakdown.md` §3)。

## Install

```toml
[dependencies]
fizz_thinking_cue_detector = { git = "https://github.com/aiviecast/fizz-thinking-cue-detector", tag = "v0.1.0" }
```

## Tests

```bash
almide test
```

純ロジックなのでネットワーク・API キー不要でテストできる。
