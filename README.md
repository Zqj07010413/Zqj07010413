<form action="submit.php" method="POST">

```
<h2>一、長輩資料</h2>

<label>長輩姓名</label>
<input type="text" name="elderly_name" required>

<label>長輩性別</label>
<select name="elderly_gender" required>
    <option value="">請選擇</option>
    <option value="男">男</option>
    <option value="女">女</option>
    <option value="其他">其他</option>
</select>

<label>長輩年齡</label>
<input type="number" name="elderly_age" min="0" max="120" required>

<label>目前主要居住哪個地方（路段）</label>
<input type="text" name="elderly_area">

<label>長輩的興趣愛好</label>
<textarea name="elderly_hobbies"></textarea>


<h2>二、家屬資料</h2>

<label>家屬姓名</label>
<input type="text" name="family_name" required>

<label>家屬電話</label>
<input type="tel" name="family_phone" required>

<label>和長輩的關係</label>
<select name="relationship" required>
    <option value="">請選擇</option>
    <option value="子女">子女</option>
    <option value="配偶">配偶</option>
    <option value="兄弟姊妹">兄弟姊妹</option>
    <option value="其他親屬">其他親屬</option>
    <option value="其他">其他</option>
</select>


<h2>三、長照評估資料</h2>

<label>是否有打 1966 做評估過</label>
<select name="assessment_1966" required>
    <option value="">請選擇</option>
    <option value="是">是</option>
    <option value="否">否</option>
    <option value="不確定">不確定</option>
</select>

<label>評估後等級是幾級</label>
<select name="assessment_level">
    <option value="">請選擇</option>
    <option value="第1級">第1級</option>
    <option value="第2級">第2級</option>
    <option value="第3級">第3級</option>
    <option value="第4級">第4級</option>
    <option value="第5級">第5級</option>
    <option value="第6級">第6級</option>
    <option value="第7級">第7級</option>
    <option value="第8級">第8級</option>
    <option value="尚未評估">尚未評估</option>
</select>

<label>個管師單位</label>
<input type="text" name="case_manager_unit">


<h2>四、參訪預約</h2>

<label>想預約時間日期</label>
<input type="date" name="visit_date" required>

<label>方便參觀時間</label>
<select name="visit_time" required>
    <option value="">請選擇</option>
    <option value="09:00-10:00">09:00-10:00</option>
    <option value="10:00-11:00">10:00-11:00</option>
    <option value="14:00-15:00">14:00-15:00</option>
    <option value="15:00-16:00">15:00-16:00</option>
</select>

<br><br>

<button type="submit">送出參訪預約</button>
```

</form>

