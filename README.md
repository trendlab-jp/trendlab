<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>TRENDLAB｜Xで話題のトレンドをわかりやすく解説</title>

<meta name="description" content="X（旧Twitter）で話題になっているニュースやトレンドをわかりやすく解説するTRENDLAB。今なぜ話題なのか、元ネタや世間の反応を紹介します。">

<style>

* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family:
        -apple-system,
        BlinkMacSystemFont,
        "Hiragino Kaku Gothic ProN",
        "Yu Gothic",
        Meiryo,
        sans-serif;

    background: #f4f6f8;
    color: #222;
}

a {
    color: inherit;
    text-decoration: none;
}

/* ヘッダー */

header {
    background: #111827;
    color: white;
    position: sticky;
    top: 0;
    z-index: 100;
}

.header-inner {
    max-width: 1100px;
    margin: auto;
    padding: 16px 20px;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 25px;
    font-weight: 800;
    letter-spacing: 1px;
}

.logo span {
    color: #60a5fa;
}

.menu {
    font-size: 14px;
}

/* メインビジュアル */

.hero {
    background:
        linear-gradient(135deg, #111827, #1d4ed8);

    color: white;
    padding: 65px 20px;
}

.hero-inner {
    max-width: 1100px;
    margin: auto;
}

.hero-label {
    display: inline-block;
    background: rgba(255,255,255,0.15);
    padding: 7px 13px;
    border-radius: 30px;
    font-size: 13px;
    margin-bottom: 15px;
}

.hero h1 {
    font-size: 42px;
    line-height: 1.3;
    margin: 0 0 18px;
}

.hero p {
    font-size: 16px;
    line-height: 1.8;
    max-width: 650px;
    color: #e5e7eb;
}

/* コンテナ */

.container {
    max-width: 1100px;
    margin: auto;
    padding: 35px 20px;
}

/* トレンド */

.trend-section {
    margin-top: -25px;
}

.trend-panel {
    background: white;
    border-radius: 16px;
    padding: 25px;

    box-shadow: 0 8px 30px rgba(0,0,0,0.08);
}

.section-title {
    display: flex;
    justify-content: space-between;
    align-items: center;

    margin-bottom: 20px;
}

.section-title h2 {
    margin: 0;
    font-size: 22px;
}

.update {
    font-size: 12px;
    color: #888;
}

.trend-item {
    display: flex;
    align-items: center;

    padding: 16px 5px;
    border-bottom: 1px solid #eee;
}

.trend-item:last-child {
    border-bottom: none;
}

.rank {
    font-size: 20px;
    font-weight: bold;
    width: 45px;
    color: #2563eb;
}

.trend-content {
    flex: 1;
}

.trend-name {
    font-weight: bold;
    font-size: 16px;
}

.trend-info {
    margin-top: 5px;
    font-size: 12px;
    color: #888;
}

.hot {
    color: #ef4444;
    font-weight: bold;
    font-size: 12px;
}

/* カテゴリー */

.categories {
    display: flex;
    gap: 10px;
    overflow-x: auto;
    padding-bottom: 5px;
}

.category {
    background: white;
    border: 1px solid #e5e7eb;

    padding: 10px 16px;
    border-radius: 30px;

    white-space: nowrap;
    font-size: 13px;
}

.category:hover {
    background: #eff6ff;
}

/* 記事 */

.articles {
    display: grid;
    grid-template-columns:
        repeat(2, 1fr);

    gap: 20px;
}

.article {
    background: white;
    border-radius: 14px;
    overflow: hidden;

    box-shadow:
        0 4px 15px rgba(0,0,0,0.05);
}

.article-image {
    height: 150px;

    background:
        linear-gradient(
            135deg,
            #dbeafe,
            #bfdbfe
        );

    display: flex;
    align-items: center;
    justify-content: center;

    font-size: 45px;
}

.article-body {
    padding: 20px;
}

.tag {
    display: inline-block;

    background: #eff6ff;
    color: #2563eb;

    padding: 5px 10px;

    border-radius: 20px;

    font-size: 11px;
    font-weight: bold;
}

.article h3 {
    margin: 12px 0;

    font-size: 18px;
    line-height: 1.5;
}

.article p {
    color: #666;
    font-size: 13px;
    line-height: 1.7;
}

.article-date {
    font-size: 11px;
    color: #999;
}

/* アフィリエイト */

.recommend {
    background: white;
    border-radius: 14px;

    padding: 25px;
    margin-top: 20px;

    border: 1px solid #e5e7eb;
}

.recommend h3 {
    margin-top: 0;
}

.recommend-box {
    background: #f8fafc;

    padding: 18px;
    border-radius: 10px;

    margin-top: 15px;
}

.button {
    display: inline-block;

    background: #2563eb;
    color: white;

    padding: 12px 20px;

    border-radius: 8px;

    font-weight: bold;
    font-size: 13px;

    margin-top: 10px;
}

/* フッター */

footer {
    background: #111827;
    color: #9ca3af;

    margin-top: 40px;
    padding: 40px 20px;
}

.footer-inner {
    max-width: 1100px;
    margin: auto;
}

.footer-logo {
    color: white;
    font-size: 22px;
    font-weight: bold;
}

.footer-links {
    margin-top: 20px;
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
    font-size: 13px;
}

.copyright {
    margin-top: 25px;
    font-size: 11px;
}

/* スマホ */

@media (max-width: 700px) {

    .hero {
        padding: 50px 20px;
    }

    .hero h1 {
        font-size: 32px;
    }

    .articles {
        grid-template-columns: 1fr;
    }

    .article-image {
        height: 130px;
    }

    .trend-panel {
        padding: 20px;
    }
}

</style>
</head>

<body>

<!-- ヘッダー -->

<header>

<div class="header-inner">

<div class="logo">
TREND<span>LAB</span>
</div>

<div class="menu">
Xトレンド解説メディア
</div>

</div>

</header>


<!-- メインビジュアル -->

<section class="hero">

<div class="hero-inner">

<div class="hero-label">
🔥 X TREND MEDIA
</div>

<h1>
Xで話題の<br>
「なぜ？」をわかりやすく。
</h1>

<p>
X（旧Twitter）で今話題になっているニュースや
キーワードをピックアップ。
なぜトレンドになったのか、何が起きたのかを
わかりやすく解説します。
</p>

</div>

</section>


<!-- トレンド -->

<section class="container trend-section">

<div class="trend-panel">

<div class="section-title">

<h2>
🔥 今日のXトレンド
</h2>

<div class="update">
最終更新：本日
</div>

</div>


<div class="trend-item">

<div class="rank">
01
</div>

<div class="trend-content">

<div class="trend-name">
話題のニュース
</div>

<div class="trend-info">
ニュース・話題
</div>

</div>

<div class="hot">
🔥 HOT
</div>

</div>


<div class="trend-item">

<div class="rank">
02
</div>

<div class="trend-content">

<div class="trend-name">
話題のAIサービス
</div>

<div class="trend-info">
AI・テクノロジー
</div>

</div>

<div class="hot">
🔥 HOT
</div>

</div>


<div class="trend-item">

<div class="rank">
03
</div>

<div class="trend-content">

<div class="trend-name">
新作ゲーム
</div>

<div class="trend-info">
ゲーム
</div>

</div>

<div class="hot">
🔥 HOT
</div>

</div>


<div class="trend-item">

<div class="rank">
04
</div>

<div class="trend-content">

<div class="trend-name">
人気アニメ
</div>

<div class="trend-info">
エンタメ
</div>

</div>

</div>


<div class="trend-item">

<div class="rank">
05
</div>

<div class="trend-content">

<div class="trend-name">
スポーツニュース
</div>

<div class="trend-info">
スポーツ
</div>

</div>

</div>

</div>

</section>


<!-- カテゴリー -->

<section class="container">

<div class="section-title">

<h2>
カテゴリー
</h2>

</div>

<div class="categories">

<a class="category">🔥 総合</a>

<a class="category">📰 ニュース</a>

<a class="category">🎮 ゲーム</a>

<a class="category">🎬 エンタメ</a>

<a class="category">🤖 AI・IT</a>

<a class="category">⚽ スポーツ</a>

</div>

</section>


<!-- 記事 -->

<section class="container">

<div class="section-title">

<h2>
📰 最新のトレンド解説
</h2>

<div class="update">
NEW
</div>

</div>


<div class="articles">


<!-- 記事1 -->

<article class="article">

<div class="article-image">
📰
</div>

<div class="article-body">

<span class="tag">
NEWS
</span>

<h3>
「話題のニュース」がXでトレンド入り！一体何があった？
</h3>

<p>
Xで突然話題になったニュースについて、
なぜトレンド入りしたのか、
元ネタや背景をわかりやすく解説します。
</p>

<div class="article-date">
2026.08.18
</div>

</div>

</article>


<!-- 記事2 -->

<article class="article">

<div class="article-image">
🤖
</div>

<div class="article-body">

<span class="tag">
AI・TECH
</span>

<h3>
いまXで話題のAIとは？注目されている理由を解説
</h3>

<p>
話題になっているAIサービスについて、
何ができるのか、どんな特徴があるのかを
初心者にもわかりやすく紹介します。
</p>

<div class="article-date">
2026.08.18
</div>

</div>

</article>


<!-- 記事3 -->

<article class="article">

<div class="article-image">
🎮
</div>

<div class="article-body">

<span class="tag">
GAME
</span>

<h3>
新作ゲームがXで話題！発売日や注目ポイントを紹介
</h3>

<p>
SNSで注目されているゲームについて、
なぜ人気なのか、どんなゲームなのかを
詳しく紹介します。
</p>

<div class="article-date">
2026.08.18
</div>

</div>

</article>


<!-- 記事4 -->

<article class="article">

<div class="article-image">
🎬
</div>

<div class="article-body">

<span class="tag">
ENTERTAINMENT
</span>

<h3>
人気作品がトレンド入り！SNSで話題になった理由とは？
</h3>

<p>
Xで話題になっている作品について、
話題になったきっかけやSNSでの反応を
紹介します。
</p>

<div class="article-date">
2026.08.18
</div>

</div>

</article>

</div>

</section>


<!-- おすすめ -->

<section class="container">

<div class="recommend">

<h2>
🛍 TRENDLABおすすめ
</h2>

<p>
トレンドをきっかけに、
実際に使ってみたいサービスや商品を紹介します。
</p>


<div class="recommend-box">

<h3>
話題の商品・サービスをチェック
</h3>

<p>
TRENDLABでは、話題になっている
商品・サービスの情報も紹介していきます。
</p>

<!-- 後でアフィリエイトリンクを設置 -->

<a href="#" class="button">
おすすめを見る →
</a>

</div>

</div>

</section>


<!-- フッター -->

<footer>

<div class="footer-inner">

<div class="footer-logo">
TRENDLAB
</div>

<div class="footer-links">

<a href="#">
サイトについて
</a>

<a href="#">
お問い合わせ
</a>

<a href="#">
プライバシーポリシー
</a>

</div>

<div class="copyright">

© 2026 TRENDLAB All Rights Reserved.

</div>

</div>

</footer>


</body>
</html>
