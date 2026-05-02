# Pages


curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/i
nstall.sh

```

**情報源:**
*   Node.js 公式サイト (nodejs.org)
*   nvm GitHub リポジトリ (github.com/nvm-sh/nvm)
*   NodeSource ディストリビューションガイド

> **注意:** 質問に対する答えが見つからない場合は正直に申告するよう承っておりますが、今回はUbuntuにNode.jsとnpmをインストールする方法はいくつかありますが、最も推奨されるのはバージョン管理ツール（**nvm**）を使用する方法、または公式のリポジトリから安定版を導入する方法です。

---

## 1. 推奨：nvm (Node Version Manager) を使う方法
複数のプロジェクトで異なるバージョンを使い分けたい場合や、権限トラブルを避けたい場合に最も適しています。K

1.  **インストールスクリプトの実行**
    ```bash
    curl -o- [https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh](https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh) | bash
    ```
2.  **設定の反映**
    端末を再起動するか、以下のコマンドを実行します。
    ```bash
    source ~/.bashrc
    ```
3.  **Node.jsのインストール**
    最新のLTS（推奨版）をインストールします。npmも自動的に同梱されます。
    ```bash
    nvm install --lts
    ```

---

## 2. 標準的な方法：Ubuntu公式リポジトリを使う方法
手軽ですが、Node.jsのバージョンが古い場合があります。
```bash
sudo apt update
sudo apt install nodejs npm
```

---

## 3. 特定の最新版を入れたい場合：NodeSourceを使う方法
最新のメジャーバージョン（例：Node.js 20.xなど）を直接指定して導入できます。

1.  **セットアップスクリプトの実行**（Node.js 20の場合）
    ```bash
    curl -fsSL [https://deb.nodesource.com/setup_20.x](https://deb.nodesource.com/setup_20.x) | sudo -E bash -
    ```
2.  **インストール**
    ```bash
    sudo apt-get install -y nodejs
    ```

---

## インストールの確認
正しくインストールされたか、バージョンを表示して確認してください。

```bash
node -v
npm -v
```

**情報源:**
*   Node.js 公式サイト (nodejs.org)
*   nvm GitHub リポジトリ (github.com/nvm-sh/nvm)
*   NodeSource ディストリビューションガイド

> **注意:** 質問に対する答えが見つからない場合は正直に申告するよう承っておりますが、今回は公式ドキュメントおよび標準的な手順に基づき回答いたしました。もしインストール中にエラーが出る場合は、エラーメッセージを教えていただければさらに詳しくお調べします。
```

目指すホームページ

見やすい、使いやすい、分かりやすい、必要な情報にアクセスしやすい

サイトの構造を瞬時に理解することができる。

必要な情報にアクセスするというよりは、探索を楽しんでもらう

[homepage](https://keio-sf-society.github.io/Pages/)

<!-- <aside class="sidebar">
      <h2>Menu</h2>
      <nav class="sidebar-nav">p
        <ul>
          <li><a href="#">ダッシュボード</a></li>
          <li><a href="#">マイページ</a></li>
          <li><a href="#">設定</a></li>
        </ul>
      </nav>
    </aside> -->

```htm
<!DOCTYPE html>
<html lang="ja">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>慶應義塾大学SF研究会</title>
	<style>
		:root {
			--bg-color: #0d1117; /* GitHubダークモード風 */
			--card-bg: #161b22;
			--text-color: #e6edf3;
			--accent-color: #58a6ff;
			--secondary-text: #8b949e;
		}

		body {
			background-color: var(--bg-color);
			color: var(--text-color);
			font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
			margin: 0;
			padding: 2rem;
			line-height: 1.6;
		}

        header {
            text-align: center;
            margin-bottom: 3rem;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        .subtitle {
            color: var(--secondary-text);
            font-size: 1.1rem;
        }

        /* 2. Bento Grid（弁当グリッド）レイアウト */
        .container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            max-width: 1000px;
            margin: 0 auto;
        }

        .card {
            background-color: var(--card-bg);
            border: 1px solid #30363d;
            border-radius: 16px;
            padding: 1.5rem;
            transition: transform 0.2s ease, border-color 0.2s ease;
        }

        /* ホバー時のマイクロインタラクション */
        .card:hover {
            transform: translateY(-5px);
            border-color: var(--accent-color);
        }

        /* 特定のカードを大きく見せる（強調） */
        .card-large {
            grid-column: span 2;
        }

        h2 {
            margin-top: 0;
            color: var(--accent-color);
            font-size: 1.25rem;
        }

        .tag {
            display: inline-block;
            background: #238636;
            color: white;
            font-size: 0.75rem;
            padding: 2px 8px;
            border-radius: 20px;
            margin-bottom: 0.5rem;
        }

        /* レスポンシブ対応（スマホでは1列に） */
        @media (max-width: 768px) {
            .card-large {
                grid-column: span 1;
            }
        }
    </style>
</head>

<body>
	<header>
		<h1>慶應義塾大学SF研究会</h1>
		<p class="subtitle">慶應義塾大学SF研究会の公式ウェブサイトです。</p>
	</header>

    <main class="container">
        <div class="card card-large">
            <span class="tag">About</span>
            <h2>自己紹介 / コンセプト</h2>
            <p>ここにサイトの核となるメッセージや、あなたのバックグラウンドを記述します。Bento Gridを採用することで、情報の優先順位が直感的に伝わります。</p>
        </div>

        <div class="card">
            <span class="tag">Project</span>
            <h2>開発実績 A</h2>
            <p>GitHub APIを活用した動的なダッシュボードの構築例など。</p>
        </div>

        <div class="card">
            <span class="tag">Project</span>
            <h2>開発実績 B</h2>
            <p>静的サイトジェネレーターを用いた高速なドキュメント作成。</p>
        </div>

        <div class="card">
            <span class="tag">Skills</span>
            <h2>使用技術</h2>
            <p>HTML / CSS / JavaScript / Git / LaTeX</p>
        </div>

        <div class="card">
            <span class="tag">Contact</span>
            <h2>リンク</h2>
            <p><a href="#" style="color: var(--accent-color); text-decoration: none;">→ GitHub Profile</a></p>
            <p><a href="#" style="color: var(--accent-color); text-decoration: none;">→ Email</a></p>
        </div>
    </main>

</body>
</html>
```