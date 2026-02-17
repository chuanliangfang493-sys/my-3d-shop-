<!DOCTYPE html>
<html lang="zh">
<head>
  <meta charset="UTF-8" />
  <title>商品 3D 展示 · 下单页面</title>
  <meta name="ビーズ" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      margin: 0;
      padding: 20px;
      background: #f5f5f5;
    }
    .container {
      max-width: 900px;
      margin: auto;
      background: #fff;
      padding: 20px;
      border-radius: 8px;
    }
    h1 {
      margin-top: 0;
    }
    iframe {
      width: 100%;
      height: 400px;
      border: none;
      border-radius: 8px;
      background: #000;
    }
    form {
      margin-top: 30px;
    }
    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }
    input, textarea, button {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      font-size: 16px;
    }
    button {
      margin-top: 20px;
      background: #007aff;
      color: white;
      border: none;
      border-radius: 6px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>商品名称（这里改）</h1>
    <p>商品简单介绍，可写规格、成色、价格等。</p>

    <!-- 3D展示区域 -->
    <iframe 
      src="这里放3D链接"
      allowfullscreen>
    </iframe>

    <!-- 下单表单 -->
    <form action="https://formsubmit.co/你的邮箱@example.com" method="POST">
      <label>姓名</label>
      <input type="text" name="name" required>

      <label>联系方式（微信 / LINE / 电话）</label>
      <input type="text" name="contact" required>

      <label>数量</label>
      <input type="number" name="quantity" value="1" min="1">

      <label>备注</label>
      <textarea name="message"></textarea>

      <button type="submit">提交订单</button>
    </form>
  </div>
</body>
</html>
