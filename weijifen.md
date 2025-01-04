---
title: weijifen
date: 2024-12-22 16:11:41
tags:
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Auto Resize iframe</title>
</head>
<body>
    <iframe id="weijifenmd" src="norender/weijifenmd.html" frameborder="0" style="width: 100%;"></iframe>

    <script>
        function resizeIframe() {
            var iframe = document.getElementById('weijifenmd');
            iframe.style.height = iframe.contentWindow.document.body.scrollHeight + 'px';
        }

        // 调整iframe大小的函数将在iframe加载内容后调用
        document.getElementById('weijifenmd').onload = function() {
            resizeIframe();
        };
    </script>
</body>
</html>
