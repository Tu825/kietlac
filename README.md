<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>🌈 Ảnh Xoay & Chữ Đẹp</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      color: #fff;
      text-align: center;
      padding: 50px;
      overflow-x: hidden;
    }
    .image-container {
      margin: auto;
      width: 320px;
      height: 320px;
      border-radius: 50%;
      border: 6px solid #fff;
      box-shadow: 0 0 30px #f0f;
      animation: spin 25s linear infinite;
    }
    .image-container img {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      object-fit: cover;
    }
    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
    .caption {
      margin-top: 40px;
      font-size: 28px;
      font-weight: bold;
      cursor: pointer;
      background: linear-gradient(90deg, #ff6ec4, #7873f5);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      transition: transform 0.3s ease;
    }
    .caption:hover {
      transform: scale(1.1);
    }
    .hidden-text {
      margin-top: 20px;
      font-size: 20px;
      padding: 10px 20px;
      border-radius: 12px;
      display: none;
      color: white;
      background: linear-gradient(135deg, #ff416c, #ff4b2b);
      box-shadow: 0 0 20px rgba(255, 75, 43, 0.5);
      animation: fadeIn 0.5s ease;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <div class="image-container">
    <img src="https://sf-static.upanhlaylink.com/img/image_202507155093659ecb26f1657ac3bb08ed4e072c.jpg" alt="Ảnh người dùng">
  </div>

  <div class="caption" onclick="toggleText()">
    🌟 Tôi có điều muốn nói với bạn...
  </div>

  <div class="hidden-text" id="hiddenText">
    💌 Bạn có thể làm ghệ tôi chứ? :3333333333
  </div>

  <script>
    function toggleText() {
      const text = document.getElementById('hiddenText');
      text.style.display = text.style.display === 'block' ? 'none' : 'block';
    }
  </script>
</body>
</html>
