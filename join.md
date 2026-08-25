---
layout: default
title: タビカケへの招待
permalink: /join
---

# タビカケへの招待

<div id="invite-card" style="padding:20px;border:1px solid #eadfd6;border-radius:18px;background:#fffaf5;">
  <p id="invite-kind" style="font-weight:700;color:#e07a5f;">招待内容を読み込んでいます…</p>
  <p style="margin-bottom:6px;">招待コード</p>
  <p id="invite-code" style="font-size:28px;font-weight:800;letter-spacing:3px;margin-top:0;user-select:all;">--------</p>
  <button id="copy-code" type="button" style="border:0;border-radius:999px;padding:11px 18px;background:#e07a5f;color:white;font-weight:700;">コードをコピー</button>
</div>

## 参加方法

1. タビカケを開く
2. 下部の「共有」タブを開く
3. 「コードで参加」を選ぶ
4. 上の招待コードを入力する

<p><a href="https://apps.apple.com/app/id6779487027">App Storeでタビカケを開く</a></p>

<script>
  (function () {
    var params = new URLSearchParams(window.location.search);
    var type = params.get('type');
    var code = (params.get('code') || '').toUpperCase().replace(/[^A-Z0-9]/g, '').slice(0, 32);
    var kind = type === 'circle' ? 'サークルへの招待' : '共有ブックへの招待';
    document.getElementById('invite-kind').textContent = kind;
    document.getElementById('invite-code').textContent = code || 'コードがありません';
    document.getElementById('copy-code').addEventListener('click', function () {
      if (!code) return;
      navigator.clipboard.writeText(code).then(function () {
        document.getElementById('copy-code').textContent = 'コピーしました';
      });
    });
  })();
</script>
