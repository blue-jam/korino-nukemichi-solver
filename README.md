# こおりのぬけみちソルバー (Sliding Floor Puzzle Solver)

ポケットモンスター金・銀に出てくる、氷の床で滑るパズルゲームのソルバーです。このプロジェクトは、パズルを解くアルゴリズムと手動でプレイできるUIの両方を提供するHTML SPAです。

## 🎮 遊び方

[GitHub Pages](https://blue-jam.github.io/korino-nukemichi-solver/)でプレイできます。

## 📝 パズルの記法

パズルは以下の文字を使ってグリッド形式で表現されます：

- `#` - 壁・岩 (Wall/Rock)
- `_` - 滑る床 (Ice/Sliding Floor) - この上を移動すると、壁や普通の床に当たるまで滑り続けます
- `.` - 普通の床 (Normal Floor) - 滑らずに止まれます
- `S` - スタート (Start)
- `G` - ゴール (Goal)

### パズル例

```
#####
#S__#
#.#.#
#__G#
#####
```

## ✨ 機能

1. **パズルソルバー** - BFS（幅優先探索）アルゴリズムを使用して最短経路を見つけます
2. **経路の可視化** - 解が見つかった場合、パスを黄色でハイライト表示します
3. **手動プレイモード** - マウスまたはキーボードの矢印キーでパズルをプレイできます

## 🚀 ローカルで実行

```bash
# リポジトリをクローン
git clone https://github.com/blue-jam/korino-nukemichi-solver.git
cd korino-nukemichi-solver

# ローカルサーバーを起動
python3 -m http.server 8000

# ブラウザで http://localhost:8000 を開く
```

## 🔧 技術スタック

- HTML5
- CSS3 (グラデーション、アニメーション)
- JavaScript (ES6+)
- GitHub Actions (自動デプロイ)

## 📄 ライセンス

Apache License 2.0