# @airiah7 - スポイトの色を保存

AviUtl ExEdit2 (AviUtl2) 用の汎用プラグイン (`.aux2`) です。
スポイトで取得した色を **保存・更新・削除・微調整** できるウィジェットを追加します。

※デフォルトのスポイト機能では、取得した色を使いまわせる機能がありません

<p align="center">
  <img src="https://img.shields.io/badge/AviUtl2-AviUtlExEdit2-blue">
  <img src="https://img.shields.io/badge/plugin-.aux2-green">
</p>

---

## 主な機能

- **スポイト**: 画面上の任意のピクセルから色を取得
- **保存**: 取得・編集した色を名前 (保存名) 付きで一覧に登録
- **編集**: HEX (カラーコード) / R / G / B を相互連動で微調整 (プレビュー付き)
- 登録した色は自動保存されます。

---

## インストール

1. [Releases](https://github.com/airiah7/airiah7--aviutl2--plugin--picked-color-storage/releases) から `airiah7__picked_color_storage.aux2` をダウンロード
2. AviUtl2 のプラグインフォルダに配置

3. AviUtl2 を再起動し、 `表示` > `@airiah7 - スポイトの色を保存` にチェックを入れる

※プラグインフォルダは、AviUtl2を起動してから `その他` > `アプリケーションデータ` > `プラグインフォルダ` で見つかります。

---

## 使い方

| 操作 | 内容 |
|---|---|
| スポイト | ボタンを押し、画面上をクリックで色取得 (Esc で中止) |
| 追加 | 現在の色を保存名付きで一覧へ登録 |
| 更新 | 選択中の項目を現在の色・保存名で上書き |
| 削除 | 選択中の項目を削除 |
| HEX / R / G / B | 数値を直接編集 (相互に連動) |
| 一覧クリック | 編集対象として読み込み |

---

## 保存データ

登録した色は、プラグインと同じ場所に自動生成される以下のファイルへ保存されます。

```
settings\airiah7__picked_color_storage\color.txt
```

- 文字コード: UTF-8 (BOM 付き)
- 形式: 1 行 1 色 `rrggbb,保存名`

他プラグインと衝突しないよう、専用フォルダ・ファイル名にしています。

---

## ライセンス

MIT License — Copyright (c) 2026 airiah7
