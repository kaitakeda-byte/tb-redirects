# tb-redirects

業務スプシ等への redirect ページ集. 用途: **ブックマークバーに独自 favicon を表示** するため。

## 構造

`docs/` を GitHub Pages の root として publish.

| URL | Redirect先 | favicon |
|---|---|---|
| `/us.html` | USデイリー請求書作成FMT | ティール「US」 |

## 追加方法

1. `docs/<name>.html` 作成 (=`us.html` をテンプレに)
2. favicon SVG → base64 を `<link rel="icon">` に埋め込み
3. `<meta http-equiv="refresh">` + `window.location.replace` で redirect
4. `docs/index.html` に追記
