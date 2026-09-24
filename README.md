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
      font-size: 16px;
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
      color: #655448;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 12px 14px;
      border: 1px solid #dccdbb;
      border-radius: 12px;
      background: #fff;
      font-size: 16px;
      font-family: inherit;
    }

    textarea {
      min-height: 90px;
      resize: vertical;
    }

    input:focus,
    select:focus,
    textarea:focus {
      outline: none;
      border-color: #c99d68;
    }

    .submit-area {
      text-align: center;
      margin-top: 25px;
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
    }

    button:hover {
      background: #b98b57;
    }

    button:disabled {
      background: #c8b8a6;
      cursor: not-allowed;
    }

    #message {
      display: none;
      margin-top: 18px;
      padding: 14px;
      border-radius: 12px;
      text-align: center;
      line-height: 1.6;
    }

    .success {
      background: #edf5e9;
      color: #55704d;
    }

    .error {
      background: #f8e8e4;
      color: #8a4d43;
    }

    .footer {
      text-align: center;
      color: #8b7a6b;
      font-size: 14px;
      line-height: 1.8;
      margin-top: 25px;
    }

    @media (max-width: 600px) {
      .container {
        margin: 15px auto;
        padding: 12px;
      }

      .header {
        padding: 28px 18px;
      }

      .header h1 {
        font-size: 24px;
      }

      .card {
        padding: 22px 18px;
      }
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

  <!--
    這裡就是 Google Apps Script 的網址
  -->

  <form
    id="reservationForm"
    action="https://script.google.com/macros/s/AKfycbzf7ttVtqMNnTXvp9W25sgWjx7N1XxVWJF2CVHt5RFEMcrHsZ-4xZ9VCd9FmS_x544F/exec"
    method="POST"
    target="hidden_iframe"
  >

```
<div class="card">

  <h2>👴 長輩基本資料</h2>

  <label for="elderly_name">長輩姓名</label>
  <input
    type="text"
    id="elderly_name"
    name="elderly_nam_
```
