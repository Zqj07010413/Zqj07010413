html
<!DOCTYPE html>
<html lang="zh-Hant">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>台北市私立六十三社區長照機構｜參訪預約</title>

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            font-family: "Microsoft JhengHei", "Noto Sans TC", sans-serif;
            background: #f8f3e9;
            color: #51483f;
            line-height: 1.8;
        }

        .hero {
            background: linear-gradient(135deg, #ead8b7, #f4e9d2);
            padding: 60px 20px;
            text-align: center;
        }

        .hero h1 {
            margin: 0;
            font-size: 34px;
            color: #5d4935;
            letter-spacing: 2px;
        }

        .hero p {
            margin: 15px auto 0;
            max-width: 700px;
            font-size: 18px;
            color: #705f4c;
        }

        .container {
            max-width: 850px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .intro {
            background: #fffdf8;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 5px 20px rgba(100, 80, 50, 0.08);
            margin-bottom: 30px;
        }

        .intro h2 {
            margin-top: 0;
            color: #806348;
        }

        .form-card {
            background: #fffdf8;
            padding: 35px;
            border-radius: 20px;
            box-shadow: 0 5px 20px rgba(100, 80, 50, 0.08);
        }

        h2 {
            margin-top: 35px;
            padding-bottom: 8px;
            border-bottom: 2px solid #ead8b7;
            color: #806348;
        }

        h2:first-child {
            margin-top: 0;
        }

        label {
            display: block;
            margin-top: 18px;
            margin-bottom: 6px;
            font-weight: bold;
            color: #5d5145;
        }

        input,
        select,
        textarea {
            width: 100%;
            padding: 13px 14px;
            border: 1px solid #d8cbb8;
            border-radius: 10px;
            background: #fff;
            font-size: 16px;
            font-family: inherit;
            color: #51483f;
        }

        input:focus,
        select:focus,
        textarea:focus {
            outline: none;
            border-color: #b89b70;
            box-shadow: 0 0 0 3px rgba(184, 155, 112, 0.15);
        }

        textarea {
            min-height: 100px;
            resize: vertical;
        }

        button {
            width: 100%;
            margin-top: 30px;
            padding: 15px;
            border: none;
            border-radius: 12px;
            background: #9b7b55;
            color: white;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            font-family: inherit;
        }

        button:hover {
            background: #806348;
        }

        button:disabled {
            background: #c5b9a8;
            cursor: wait;
        }

        .footer {
            text-align: center;
            padding: 30px 20px;
            color: #817466;
            font-size: 14px;
        }

        @media (max-width: 600px) {
            .hero {
                padding: 45px 18px;
            }

            .hero h1 {
                font-size: 26px;
            }

            .hero p {
                font-size: 16px;
            }

            .form-card,
            .intro {
                padding: 22px;
            }
        }
    </style>
</head>

<body>

<section class="hero">
    <h1>台北市私立六十三社區長照機構</h1>

    <p>日照機構｜參訪預約</p>

    <p>用心陪伴每一段生活，讓照顧更安心。</p>
</section>


<div class="container">

    <section class="intro">

        <h2>歡迎來到六十三社區長照機構</h2>

        <p>
            歡迎長輩與家屬預約參訪，
            讓我們一起認識機構環境、了解日間照顧服務，
            找到適合長輩的照顧方式。
        </p>

        <p>
            填寫以下資料後，我們將依照您提供的參訪日期與時間，
            協助安排後續參訪事宜。
        </p>

    </section>


    <section class="form-card">

        <form id="reservationForm">

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

            <input
                type="number"
                name="elderly_age"
                min="0"
                max="120"
                required
            >


            <label>目前主要居住哪個地方（路段）</label>

            <input
                type="text"
                name="elderly_area"
            >


            <label>長輩的興趣愛好</label>

            <textarea
                name="elderly_hobbies"
                placeholder="例如：唱歌、散步、下棋、種花、聊天等"
            ></textarea>



            <h2>二、家屬資料</h2>


            <label>家屬姓名</label>

            <input
                type="text"
                name="family_name"
                required
            >


            <label>家屬電話</label>

            <input
                type="tel"
                name="family_phone"
                required
            >


            <label>和長輩的關係</label>

            <select
                name="relationship"
                required
            >
                <option value="">請選擇</option>
                <option value="子女">子女</option>
                <option value="配偶">配偶</option>
                <option value="兄弟姊妹">兄弟姊妹</option>
                <option value="其他親屬">其他親屬</option>
                <option value="其他">其他</option>
            </select>



            <h2>三、長照評估資料</h2>


            <label>是否有打 1966 做評估過</label>

            <select
                name="assessment_1966"
                required
            >
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

                <option value="尚未評估">
                    尚未評估
                </option>

            </select>


            <label>個管師單位</label>

            <input
                type="text"
                name="case_manager_unit"
            >



            <h2>四、參訪預約</h2>


            <label>想預約時間日期</label>

            <input
                type="date"
                name="visit_date"
                required
            >


            <label>方便參觀時間</label>

            <select
                name="visit_time"
                required
            >

                <option value="">請選擇</option>

                <option value="09:00-10:00">
                    09:00-10:00
                </option>

                <option value="10:00-11:00">
                    10:00-11:00
                </option>

                <option value="14:00-15:00">
                    14:00-15:00
                </option>

                <option value="15:00-16:00">
                    15:00-16:00
                </option>

            </select>


            <button
                type="submit"
                id="submitButton"
            >
                送出參訪預約
            </button>

        </form>

    </section>

</div>


<footer class="footer">

    台北市私立六十三社區長照機構<br>

    感謝您的信任，期待與您見面。

</footer>



<script>

const scriptURL =
"https://script.google.com/macros/s/AKfycby66gESI7wdjPQF3R3sFnv53kBZkqbacqrMgAYf9JSBjMyxbLnQSURonMpO-bqIZAAInA/exec";


document
.getElementById("reservationForm")
.addEventListener("submit", function(e) {

    e.preventDefault();

    const form = e.target;

    const button =
        document.getElementById("submitButton");


    button.disabled = true;

    button.textContent = "資料送出中...";


    const data = {

        elderly_name:
            form.elderly_name.value,

        elderly_gender:
            form.elderly_gender.value,

        elderly_age:
            form.elderly_age.value,

        elderly_area:
            form.elderly_area.value,

        elderly_hobbies:
            form.elderly_hobbies.value,


        family_name:
            form.family_name.value,

        family_phone:
            form.family_phone.value,

        relationship:
            form.relationship.value,


        assessment_1966:
            form.assessment_1966.value,

        assessment_level:
            form.assessment_level.value,

        case_manager_unit:
            form.case_manager_unit.value,


        visit_date:
            form.visit_date.value,

        visit_time:
            form.visit_time.value

    };


    fetch(scriptURL, {

        method: "POST",

        body: JSON.stringify(data)

    })

    .then(response => response.json())

    .then(result => {

        if (result.success) {

            alert(
                "✅ 預約資料已成功送出！\n\n" +
                "我們會再與您聯繫確認參訪時間。"
            );

            form.reset();

        } else {

            alert(
                "❌ 資料送出失敗，請稍後再試。"
            );

        }

    })

    .catch(error => {

        console.error("錯誤：", error);

        alert(
            "❌ 系統發生錯誤，資料可能沒有送出。\n\n" +
            "請稍後再試。"
        );

    })

    .finally(() => {

        button.disabled = false;

        button.textContent =
            "送出參訪預約";

    });

});

</script>


</body>
</html>




