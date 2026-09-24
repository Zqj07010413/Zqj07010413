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
  font-family: "Microsoft JhengHei", sans-serif;
  background: #f8f1e7;
  color: #5f5146;
}

.container {
  max-width: 760px;
  margin: 40px auto;
  padding: 20px;
}

.header {
  background: #e8cfae;
  border-radius: 24px;
  padding: 35px 25px;
  text-align: center;
  margin-bottom: 25px;
}

.header h1 {
  margin: 0 0 10px;
  color: #6b5544;
  font-size: 30px;
}

.header p {
  margin: 5px 0;
  line-height: 1.8;
}

.card {
  background: #fffaf4;
  border-radius: 22px;
  padding: 30px;
  margin-bottom: 20px;
  box-shadow: 0 5px 18px rgba(120, 90, 60, 0.08);
}

.card h2 {
  margin-top: 0;
  color: #725c49;
  font-size: 21px;
  border-left: 5px solid #d6ad78;
  padding-left: 10px;
}

label {
  display: block;
  margin-top: 18px;
  margin-bottom: 7px;
  font-weight: bold;
}

input,
select,
textarea {
  width: 100%;
  padding: 12px 14px;
  border: 1px solid #dccdbb;
  border-radius: 12px;
  background: white;
  font-size: 16px;
  font-family: inherit;
}

textarea {
  min-height: 90px;
  resize: vertical;
}

button {
  width: 100%;
  padding: 15px;
  border: none;
  border-radius: 15px;
  background: #c99d68;
  color: white;
  font-size: 18px;
  font-weight: bold;
  cursor: pointer;
  margin-top: 25px;
}

button:disabled {
  background: #c8b8a6;
}

#message {
  display: none;
  margin-top: 18px;
  padding: 14px;
  border-radius: 12px;
  text-align: center;
}

.success {
  display: block !important;
  background: #edf5e9;
  color: #55704d;
}

.footer {
  text-align: center;
  color: #8b7a6b;
  font-size: 14px;
  line-height: 1.8;
  margin-top: 25px;
}
</style>

</head>

<body>

<div class="container">

<div class="header">
<h1>六十三社區長照機構</h1>
<p>日照機構參訪預約</p>
<p>歡迎家屬與長輩提前預約參觀，讓我們一起了解適合長輩的照顧服務。</p>
</div>

<form
id="reservationForm"
action="https://script.google.com/macros/s/AKfycbzf7ttVtqMNnTXvp9W25sgWjx7N1XxVWJF2CVHt5RFEMcrHsZ-4xZ9VCd9FmS_x544F/exec"
method="POST"
target="hidden_iframe"
>

<div class="card">

<h2>👴 長輩基本資料</h2>

<label for="elderly_name">長輩姓名</label>
<input
type="text"
id="elderly_name"
name="elderly_name"
required

>

<label for="elderly_gender">長輩性別</label>
<select
id="elderly_gender"
name="elderly_gender"
required

>

<option value="">請選擇</option>
<option value="男">男</option>
<option value="女">女</option>
</select>

<label for="elderly_age">長輩年齡</label>
<input
type="number"
id="elderly_age"
name="elderly_age"
min="0"
max="120"
required

>

<label for="elderly_area">目前主要居住哪個地方（路段）</label>
<input
type="text"
id="elderly_area"
name="elderly_area"
placeholder="例如：台北市○○區○○路"
required

>

<label for="elderly_hobbies">長輩的興趣愛好</label>

<textarea
id="elderly_hobbies"
name="elderly_hobbies"
placeholder="例如：唱歌、聊天、散步、看電視……"
></textarea>

</div>

<div class="card">

<h2>👨‍👩‍👧 家屬資料</h2>

<label for="family_name">家屬姓名</label>
<input
type="text"
id="family_name"
name="family_name"
required

>

<label for="family_phone">家屬電話</label>
<input
type="tel"
id="family_phone"
name="family_phone"
placeholder="例如：0912345678"
required

>

<label for="relationship">和長輩的關係</label>
<select
id="relationship"
name="relationship"
required

>

<option value="">請選擇</option>
<option value="兒子">兒子</option>
<option value="女兒">女兒</option>
<option value="媳婦">媳婦</option>
<option value="女婿">女婿</option>
<option value="配偶">配偶</option>
<option value="孫子女">孫子女</option>
<option value="其他">其他</option>
</select>

</div>

<div class="card">

<h2>📋 長照評估資料</h2>

<label for="assessment_1966">是否有打 1966 做評估過</label>
<select
id="assessment_1966"
name="assessment_1966"
required

>

<option value="">請選擇</option>
<option value="是">是</option>
<option value="否">否</option>
</select>

<label for="assessment_level">評估後等級是幾級</label>
<select
id="assessment_level"
name="assessment_level"

>

<option value="">尚未評估／不知道</option>
<option value="第2級">第2級</option>
<option value="第3級">第3級</option>
<option value="第4級">第4級</option>
<option value="第5級">第5級</option>
<option value="第6級">第6級</option>
<option value="第7級">第7級</option>
<option value="第8級">第8級</option>
</select>

<label for="case_manager_unit">個管師單位</label>
<input
type="text"
id="case_manager_unit"
name="case_manager_unit"
placeholder="若沒有可留白"

>

</div>

<div class="card">

<h2>📅 參訪預約</h2>

<label for="visit_date">想預約時間日期</label>
<input
type="date"
id="visit_date"
name="visit_date"
required

>

<label for="visit_time">方便參觀時間</label>
<select
id="visit_time"
name="visit_time"
required

>

<option value="">請選擇</option>
<option value="上午">上午</option>
<option value="下午">下午</option>
</select>

<button
type="submit"
id="submitButton"

>

送出參訪預約 </button>

<div id="message"></div>

</div>

</form>

<iframe
name="hidden_iframe"
id="hidden_iframe"
style="display:none;"
></iframe>

<div class="footer">
台北市私立六十三社區長照機構(日照機構)<br>
感謝您填寫參訪預約，我們會再與您聯繫。
</div>

</div>

<script>

const form = document.getElementById("reservationForm");
const button = document.getElementById("submitButton");
const message = document.getElementById("message");

form.addEventListener("submit", function() {

button.disabled = true;
button.textContent = "資料送出中……";

message.style.display = "block";
message.className = "";
message.textContent = "資料正在送出，請稍候……";

setTimeout(function() {

message.className = "success";
message.textContent = "✅ 預約資料已送出！我們會再與您聯繫。";

button.disabled = false;
button.textContent = "送出參訪預約";

}, 2000);

});

</script>

</body>
</html>
