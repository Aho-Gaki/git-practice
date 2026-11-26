# VS Code で学ぶ Git / GitHub 実践課題

このリポジトリは、**VS Code に組み込まれている Git 機能**を使って、Git と GitHub の基本操作をひと通り体験するための課題です。
プログラミングの知識は必要ありません。扱うのは文章（Markdown）ファイルだけです。

## この課題で体験すること

| 機能 | ミッション |
| --- | --- |
| クローン・コミット・プッシュ | Mission 1 |
| 変更の破棄（Discard） | Mission 2 |
| ブランチの作成と切り替え | Mission 3 |
| ローカルでのマージ | Mission 4 |
| プルリクエスト（PR）とプル | Mission 5 |
| コミットの取り消し（Revert） | Mission 6 |
| マージコンフリクトの解消 | Mission 7 |
| `.gitignore` で機密情報を守る | Mission 8 |

---

## 事前準備

次の 3 つを用意してください。

1. **VS Code** … https://code.visualstudio.com/ からインストール
   - 日本語で使いたい場合は、拡張機能「Japanese Language Pack for Visual Studio Code」を入れて VS Code を再起動します。
2. **Git** … https://git-scm.com/ からインストール（Windows はインストーラーの設定をすべて初期値のままで OK）
3. **GitHub アカウント** … https://github.com/ で無料登録

### Git に名前とメールアドレスを登録する（最初の 1 回だけ）

コミットには「誰が変更したか」が記録されます。VS Code を開き、メニューの **ターミナル → 新しいターミナル（Terminal → New Terminal）** で画面下にターミナルを出し、次の 2 行を 1 行ずつ貼り付けて Enter を押します（`あなたの名前` などは自分のものに置き換えてください）。

```
git config --global user.name "あなたの名前"
git config --global user.email "GitHubに登録したメールアドレス"
```

---

## 自分用のリポジトリを作ってクローンする

### 1. テンプレートから自分のリポジトリを作る

1. ブラウザでこのリポジトリのページを開きます。
2. 右上の緑色のボタン **「Use this template」→「Create a new repository」** をクリックします。
3. 次のように設定します。
   - **Include all branches（すべてのブランチを含める）に必ずチェックを入れる** ← Mission 7 で使うブランチが含まれます
   - Repository name: 好きな名前（例: `my-git-practice`）
   - 公開範囲: **Private** を選ぶ
4. **「Create repository」** をクリックします。

> これで「あなた専用のコピー」が GitHub 上にできました。以降はこのコピーで自由に練習してください。

### 2. VS Code にクローンする

1. 作成した自分のリポジトリのページで、緑色の **「Code」** ボタンを押し、表示された URL（`https://github.com/...git`）をコピーします。
2. VS Code を開き、`Ctrl + Shift + P`（Mac は `Cmd + Shift + P`）でコマンドパレットを開きます。
3. `Git: クローン`（`Git: Clone`）と入力して選び、コピーした URL を貼り付けて Enter を押します。
   - GitHub へのサインインを求められたら、画面の案内に従ってブラウザでサインインを許可します。
4. 保存先のフォルダーを選ぶと、クローンが始まります。
5. 右下に「クローンしたリポジトリを開きますか？」と出たら **「開く（Open）」** を押します。
   - 「このフォルダー内のファイルの作成者を信頼しますか？」と出たら **「はい、作成者を信頼します」** を選びます。

左側のエクスプローラーに `README.md` や `MISSIONS.md` が表示されていれば成功です。

---

## 次にやること

クローンが終わったら、VS Code で **[`MISSIONS.md`](MISSIONS.md)** を開いて、Mission 1 から順番に進めてください。

> 💡 Markdown ファイルを開いた状態で `Ctrl + Shift + V`（Mac は `Cmd + Shift + V`）を押すと、見やすいプレビュー表示で読めます。
