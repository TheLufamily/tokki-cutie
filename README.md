<!DOCTYPE html>
<html lang="zh-Hant">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>兔迷 兔迷俱樂部・呂佳寯</title>
    <style>
      body {
        font-family: "Noto Sans TC", "Roboto", sans-serif;
        background-color: #fff5ef;
        margin: 0;
        padding: 0;
        color: #222;
      }

      .container {
        max-width: 1100px;
        margin: 0 auto;
        padding: 60px 20px;
      }

      .subtitle {
        text-align: center;
        color: #ff6b00;
        font-weight: 700;
        letter-spacing: 1px;
        margin-bottom: 10px;
      }

      h1 {
        text-align: center;
        font-size: 56px;
        font-weight: 900;
        letter-spacing: 1px;
        margin: 0 0 60px;
      }

      .profile-section {
        display: flex;
        flex-wrap: wrap;
        align-items: flex-start;
        gap: 40px;
      }

      /* 左側照片卡 */
      .photo-card {
        background-color: #fff;
        border-radius: 16px;
        overflow: hidden;
        flex: 1 1 340px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
      }

      .photo-card img {
        width: 100%;
        display: block;
        object-fit: cover;
      }

      .photo-card .caption {
        background-color: #fff;
        padding: 20px 24px;
        line-height: 1.6;
      }

      .photo-card .name {
        font-size: 20px;
        font-weight: 800;
        color: #000;
        display: inline-block;
      }

      .photo-card .ename {
        color: #ff6b00;
        font-weight: 700;
        margin-left: 6px;
      }

      .photo-card .title {
        color: #333;
        font-size: 15px;
        margin-top: 6px;
        font-weight: 500;
      }

      /* 右側資訊卡 */
      .info-block {
        flex: 1 1 500px;
        display: flex;
        flex-direction: column;
        gap: 20px;
      }

      .info-header {
        padding-top: 20px;
      }

      .info-header .name {
        font-size: 28px;
        font-weight: 800;
        color: #000;
        margin-bottom: 4px;
      }

      .info-header .ename {
        color: #ff6b00;
        font-weight: 700;
        letter-spacing: 1px;
      }

      .info-card {
        background-color: #fff;
        border-radius: 16px;
        padding: 40px 50px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
      }

      table {
        width: 100%;
        border-collapse: collapse;
        font-size: 16px;
        line-height: 1.8;
      }

      td {
        padding: 12px 0;
        border-bottom: 1px solid #eee2db;
        vertical-align: top;
      }

      td:first-child {
        width: 130px;
        color: #555;
        font-weight: 600;
      }

      /* Q&A 問答卡 */
      .qa-card {
        background-color: #fff;
        border-radius: 16px;
        padding: 40px 50px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
        margin-top: 40px;
      }

      .qa-card p {
        margin: 0 0 20px;
        line-height: 1.8;
        font-size: 16px;
      }

      .qa-card .question {
        color: #ff6b00;
        font-weight: 700;
      }

      .qa-card .answer {
        color: #222;
        margin-left: 1em;
        display: block;
      }

      @media (max-width: 768px) {
        .profile-section {
          flex-direction: column;
        }
        .info-card,
        .qa-card {
          padding: 30px 25px;
        }
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="subtitle">兔迷 兔迷俱樂部・呂佳寯</div>
      <h1>TOKKI CUTIE</h1>

      <div class="profile-section">
        <!-- 左側照片卡 -->
        <div class="photo-card">
          <img src="images/110417006.JPG" alt="呂佳寯" />
          <div class="caption">
            <div class="name">呂佳寯 <span class="ename">LU JIA JUN</span></div>
            <div class="title">兔迷 兔迷俱樂部</div>
          </div>
        </div>

        <!-- 右側資訊 -->
        <div class="info-block">
          <div class="info-header">
            <div class="name">呂佳寯</div>
            <div class="ename">LU JIA JUN</div>
          </div>

          <div class="info-card">
            <table>
              <tr>
                <td>暱稱</td>
                <td>兔迷 兔迷俱樂部</td>
              </tr>
                <tr>
                <td>生日(星座)</td>
                <td>5/1(金牛座)</td>
              </tr>
              <tr>
                <td>出生地／籍貫</td>
                <td>新北市</td>
              </tr>
              <tr>
                <td>興趣愛好
                <td>玩遊戲、當兔迷</td>
              </tr>  
              <tr>
                <td>喜愛啦啦隊</td>
                <td>李素泳、朴恩惠</td>
              </tr>
              <tr>
                <td>加入年份
                <td>2025</td>
              </tr>
            </table>
          </div>

          <!-- Q&A 問答卡 -->
          <div class="qa-card">
            <p>
              <span class="question">Q：你為什麼選擇關注伊斯特？</span>
              <span class="answer">因為顏值高</span>
            </p>
            <p>
              <span class="question">Q：你最重視一名球員的什麼特質？</span>
              <span class="answer">態度</span>
            </p>
            <p>
              <span class="question">Q：你希望透過這支球隊完成什麼？</span>
              <span class="answer">從 0 到 1 的過程</span>
            </p>
            <p>
              <span class="question">Q：最想要對伊斯特說的一句話</span>
              <span class="answer">我會繼續默默支持你們</span>
            </p>
          </div>
        </div>
      </div>
    </div>
  </body>
</html>
   
