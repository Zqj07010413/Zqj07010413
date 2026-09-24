```html
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>六十三社區長照機構｜參訪預約</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: "Noto Sans TC", "Microsoft JhengHei", sans-serif;
      background: #fff8ec;
      color: #5f5145;
    }

    header {
      background: #f4d9a6;
      padding: 35px 20px;
      text-align: center;
    }

    header h1 {
      margin: 0 0 10px;
      font-size: 30px;
      color: #604b3b;
    }

    header p {
      margin: 0;
      font-size: 17px;
    }

    .container {
      width: 92%;
      max-width: 800px;
      margin: 35px auto;
    }

    .card {
      background: white;
      border-radius: 20px;
      padding: 30px;
      margin-bottom: 25px;
      box-shadow: 0 5px 18px rgba(100, 75, 40, 0.08);
    }

    .card h2 {
      margin-top: 0;
      color: #76563e;
      font-size: 22px;
    }

    label {
      display: block;
      margin-top: 18px;
      margin-bottom: 8px;
      font-weight: bold;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 13px;
      border: 1px solid #ddcdb9;
      border-radius: 10px;
      font-size: 16px;
      font-family: inherit;
      background: #fffdf9;
    }

    textarea {
      min-height: 100px;
      resize: vertical;
    }

    input:focus,
    select:focus,
    textarea:focus {
      outline: none;
      border-color: #c99d62;
    }

    .required {
      color: #c66b55;
    }

    button {
      width: 100%;
      padding: 15px;
      margin-top: 25px;
      border: none;
      border-radius: 12px;
      background: #d8a45f;
      color: white;
      font-size: 18px;
      font-weight: bold;
      cursor: pointer;
    }

    button:hover {
      background: #c58e4d;
    }

    button:disabled {
      background: #cdbda9;
      cursor: not-allowed;
    }

    #message {
      display: none;
      margin-top: 20px;
      padding: 15px;
      border-radius: 10px;
      text-align: center;
      font-weight: bold;
    }

    .success {
      background: #e7f4e4;
      color: #50734b;
    }

    .error {
      background: #f9e2df;
      color: #a24d43;
    }

    footer {
      text-align: center;
      padding: 30px 20px;
      color: #887667;
      font-size: 14px;
    }

    .note {
      font-size: 14px;
      color: #887667;
      margin-top: 8px;
    }
  </style>
</head>

<body>

<header>
  <h1>台北市私立六十三社區長照機構</h1>
  <p>日照機構參訪預約</p>
</header>

<div class="container">

  <div class="card">
    <h2>🌷 歡迎參觀六十三社區長照機構</h2>

    <p>
      歡迎家屬帶著長輩認識我們的日間照顧服務。
      填寫以下資料後，我們會依照您提供的資訊進行聯繫與參訪安排。
    </p>
  </div>

  <form
    id="reservationForm"
    action="https://script.google.com/macros/s/AKfycbzqCVBLRG4ncnuJ6o5nTX5EJwetPejRONFaplgU-CSbrHkyw29w0-4ESkgzdofWPnan/exec"
    method="POST"
    target="hidden_iframe"
  >

    <div class="card">
      <h2>👵 長輩基本資料</h2>

      <label>
        長輩姓名 <span class="required">*</span>
      </label>
      <input type="text" name="elderly_name" required>

      <label>
        長輩性別 <span class="required">*</span>
      </label>
      <select name="elderly_gender" required>
        <option value="">請選擇</option>
        <option value="男">男</option>
        <option value="女">女</option>
      </select>

      <label>
        長輩年齡 <span class="required">*</span>
      </label>
      <input type="number" name="elderly_age" min="0" required>

      <label>
        目前主要居住哪個地方（路段）
      </label>
      <input
        type="text"
        name="elderly_area"
        placeholder="例如：台北市○○區○○路"
      >

      <label>
        長輩的興趣愛好
      </label>
      <textarea
        name="elderly_hobbies"
        placeholder="例如：唱歌、下棋、散步、聊天……"
      ></textarea>
    </div>

    <div class="card">
      <h2>👨‍👩‍👧 家屬資料</h2>

      <label>
        家屬姓名 <span class="required">*</span>
      </label>
      <input type="text" name="family_name" required>

      <label>
        家屬電話 <span class="required">*</span>
      </label>
      <input type="tel" name="family_phone" required>

      <label>
        和長輩的關係 <span class="required">*</span>
      </label>
      <input
        type="text"
        name="relationship"
        placeholder="例如：女兒、兒子、配偶"
        required
      >
    </div>

    <div class="card">
      <h2>📋 照顧評估資料</h2>

      <label>
        是否有打 1966 做評估過？
      </label>
      <select name="assessment_1966">
        <option value="">請選擇</option>
        <option value="是">是</option>
        <option value="否">否</option>
      </select>

      <label>
        評估後等級是幾級？
      </label>
      <select name="assessment_level">
        <option value="">請選擇</option>
        <option value="第2級">第2級</option>
        <option value="第3級">第3級</option>
        <option value="第4級">第4級</option>
        <option value="第5級">第5級</option>
        <option value="第6級">第6級</option>
        <option value="第7級">第7級</option>
        <option value="第8級">第8級</option>
        <option value="尚未評估">尚未評估</option>
        <option value="不清楚">不清楚</option>
      </select>

      <label>
        個管師單位
      </label>
      <input
        type="text"
        name="case_manager_unit"
        placeholder="若尚未有個管師可不用填"
      >
    </div>

    <div class="card">
      <h2>📅 參訪預約</h2>

      <label>
        想預約時間日期 <span class="required">*</span>
      </label>
      <input type="date" name="visit_date" required>

      <label>
        方便參觀時間 <span class="required">*</span>
      </label>
      <select name="visit_time" required>
        <option value="">請選擇</option>
        <option value="上午">上午</option>
        <option value="下午">下午</option>
      </select>

      <p class="note">
        ※ 填寫完成後按下送出，資料會傳送至機構的預約資料表。
      </p>

      <button type="submit" id="submitButton">
        送出參訪預約
      </button>

      <div id="message"></div>
    </div>

  </form>

  <iframe
    name="hidden_iframe"
    id="hidden_iframe"
    style="display:none;"
  ></iframe>

</div>

<footer>
  © 台北市私立六十三社區長照機構
</footer>

<script>
  const form = document.getElementById("reservationForm");
  const button = document.getElementById("submitButton");
  const message = document.getElementById("message");

  form.addEventListener("submit", function() {

    button.disabled = true;
    button.textContent = "資料送出中……";

    message.style.display = "none";

    setTimeout(function() {

      message.style.display = "block";
      message.className = "success";
      message.textContent =
        "✅ 預約資料已送出！我們會再與您聯繫。";

      form.reset();

      button.disabled = false;
      button.textContent = "送出參訪預約";

    }, 1500);

  });
</script>

</body>
</html>
```
