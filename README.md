# TanksGame

Unity で制作しているタンク対戦ゲームです。複数のプレイヤーと Bot が戦車を操作し、弾を撃ち合います。

## 動作環境

- Unity 6000.3.8f1
- Input System パッケージ（`Assets/InputSystem_Actions.inputactions`）

## 始め方

1. このリポジトリをクローンします。
2. Unity Hub で Unity 6000.3.8f1 をインストールします。
3. Unity Hub の「Add」からこのフォルダを開きます。
4. `Assets/Scenes/JoinScene.unity` を開いて再生します。

## シーン

| シーン | 内容 |
| --- | --- |
| `JoinScene` | プレイヤーの参加受付 |
| `MainGameScene` | 対戦のメインシーン |
| `DevelopScene` | 開発・動作確認用 |

## ディレクトリ構成

```
Assets/
├─ Models/Tanks/   戦車・ステージのモデル、音声（Unity Tanks! Tutorial アセット）
├─ Prefabs/        Player, Bot, Bullet, TankExplosion, UI
├─ Scenes/         ゲームシーン
└─ Scripts/
   ├─ Action/      移動、攻撃、チャージ、被弾、状態管理
   ├─ Bot/         Bot の制御とセンサー
   ├─ Join/        参加処理、ゲーム管理
   ├─ Player/      プレイヤー入力
   └─ UI/          UI 制御
```

## ブランチ運用

- `main`: 安定版
- `develop`: 開発の統合ブランチ
- `feature/*`: 機能ごとの作業ブランチ。`develop` から作成し、PR で `develop` にマージします。

## ライセンス・クレジット

`Assets/Models/Tanks` 配下のアセットは Unity の Tanks! Tutorial に由来します。詳細は `Assets/Models/Tanks/Tanks!_Third-PartyNotice.txt` を参照してください。
