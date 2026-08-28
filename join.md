---
layout: default
title: 旅の招待
permalink: /join
description: "受け取った招待コードで、タビカケの「みんなとの旅」やサークルに参加できます。"
---

# 招待された旅に参加

<div class="card">
  <p class="invite-kind" id="invite-kind">招待内容を読み込んでいます…</p>
  <p class="invite-label">招待コード</p>
  <p class="invite-code" id="invite-code">--------</p>
  <div class="btn-row">
    <a class="btn" id="open-app" href="#">アプリで開いて参加する</a>
    <button class="btn btn-outline" id="copy-code" type="button">コードをコピー</button>
  </div>
  <p class="note">タビカケがインストールされている端末で開いてください。</p>
</div>

## アプリが開かないときは

次の手順でも参加できます。

1. タビカケを開く
2. 下部の「旅」タブ →「ブック」を開く
3. 一番下の「招待された旅に参加」→「コードを入力」
4. 上の招待コードを入力する

## タビカケを持っていない方は

<p class="btn-row"><a class="btn btn-store" href="https://apps.apple.com/app/id6779487027"><svg viewBox="0 0 384 512" aria-hidden="true" focusable="false"><path d="M318.7 268.7c-.2-36.7 16.4-64.4 50-84.8-18.8-26.9-47.2-41.7-84.7-44.6-35.5-2.8-74.3 20.7-88.5 20.7-15 0-49.4-19.7-76.4-19.7C63.3 141.2 4 184.8 4 273.5q0 39.3 14.4 81.2c12.8 36.7 59 126.7 107.2 125.2 25.2-.6 43-17.9 75.8-17.9 31.8 0 48.3 17.9 76.4 17.9 48.6-.7 90.4-82.5 102.6-119.3-65.2-30.7-61.7-90-61.7-91.9zm-56.6-164.2c27.3-32.4 24.8-61.9 24-72.5-24.1 1.4-52 16.4-67.9 34.9-17.5 19.8-27.8 44.3-25.6 71.9 26.1 2 49.9-11.4 69.5-34.3z"/></svg>App Store でダウンロード</a></p>

インストール後、上の招待コードを控えてから同じ手順で参加してください。

<script>
  (function () {
    var params = new URLSearchParams(window.location.search);
    var type = params.get('type');
    var code = (params.get('code') || '').toUpperCase().replace(/[^A-Z0-9]/g, '').slice(0, 32);
    var kind = type === 'circle' ? 'サークルへの招待' : 'みんなとの旅への招待';
    document.getElementById('invite-kind').textContent = kind;
    document.getElementById('invite-code').textContent = code || 'コードがありません';
    var openApp = document.getElementById('open-app');
    openApp.href = code ? ('tabikake://join?code=' + code) : '#';
    document.getElementById('copy-code').addEventListener('click', function () {
      if (!code) return;
      navigator.clipboard.writeText(code).then(function () {
        document.getElementById('copy-code').textContent = 'コピーしました';
      });
    });
  })();
</script>
