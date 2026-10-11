# moNa2 v2 — キーボードのZMK設定

**分類: キーボード / キー配列・ファームウェア設定**

moNa2キーボードのZMK設定です。このリポジトリは [Arai-yt/zmk-config-moNa2-v2](https://github.com/Arai-yt/zmk-config-moNa2-v2) のフォークです。

## 目的別の入口

| 確認・変更したいこと | 場所 |
|---|---|
| キー配列 | [config/mona2.keymap](config/mona2.keymap) / [関連JSON](config/mona2.json) |
| 機種のハードウェア定義 | [boards/shields/mona2/](boards/shields/mona2/) |
| 左右の設定 | [左側](config/mona2_l.conf) / [右側](config/mona2_r.conf) |
| ジェスチャー設定 | [config/gesture/](config/gesture/) |
| 依存するZMK・モジュール | [config/west.yml](config/west.yml) |
| ビルド対象 | [build.yaml](build.yaml) / [GitHub Actionsの定義](.github/workflows/build.yml) |
| COROPITの変更手順 | [docs/COROPIT.md](docs/COROPIT.md) |
| 資料の一覧 | [docs/README.md](docs/README.md) |

## 設定・ビルドの確認

`build.yaml` は `seeeduino_xiao_ble` 向けの `mona2_r rgbled_adapter`、`mona2_l rgbled_adapter`、`settings_reset` を定義しています。
COROPITを使用する場合は [変更手順](docs/COROPIT.md) と [右側overlay](boards/shields/mona2/mona2_r.overlay) を確認します。元READMEに記載されていた変更前・変更後のコードは、専用資料にそのまま残しています。

2026-10-11の整理着手時点でmain以外のブランチ・PRは確認した一覧にありません。今回の案内整備は新しい実機検証やファームウェアのリリースを示すものではありません。
