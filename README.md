# ふーっとロウソク

2歳の子ども向け。マイクに「ふーっ」と息を吹きかけるとロウソクの炎が傾いて消え、
芯から煙が立ちのぼるアプリ。誕生日ケーキモード(1〜5本)つき。

**遊ぶ → https://ogawahari.github.io/fuutto-rousoku/**

- はじめる → マイクを「許可」→ ロウソクに息を吹きかける
- マイクが使えないときは、ロウソクをタップしても消える
- 右上の ⚙ を長押しで設定(本数 / ケーキ / マイク感度 / 音 / 自動再点火)
- ホーム画面に追加すると、全画面のアプリとして起動できる

## このリポジトリについて

ここにあるのは**ビルド済みの配信物**。ソースコードは
`ogawahari/AKAtools` の `apps/candle/`。

`main` ブランチのルートを GitHub Pages(Settings > Pages > Deploy from a branch)がそのまま配信する。
更新するときは AKAtools 側で

```bash
cd apps/candle && npx vite build --base=./
```

して `dist/` の中身(`index.html` / `assets/` / `candle-icon.svg`)を置き換える。
