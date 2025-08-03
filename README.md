<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>موقع الاقتباسات الملهمة</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    background: #f0f8ff;
    margin: 0; padding: 0;
    color: #333;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
  header {
    background: #0066cc;
    color: white;
    padding: 20px;
    text-align: center;
  }
  main {
    flex: 1;
    max-width: 700px;
    margin: 20px auto;
    padding: 0 15px;
  }
  #quote-box {
    background: white;
    border-radius: 8px;
    padding: 25px 20px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    font-size: 22px;
    line-height: 1.5;
    text-align: center;
    margin-bottom: 20px;
  }
  button {
    background: #0066cc;
    color: white;
    border: none;
    padding: 12px 25px;
    font-size: 18px;
    border-radius: 6px;
    cursor: pointer;
  }
  button:hover {
    background: #004999;
  }
  footer {
    text-align: center;
    padding: 15px 10px;
    font-size: 14px;
    color: #666;
  }
  /* Placeholder for ads */
  #ad-space {
    background: #ddd;
    color: #666;
    text-align: center;
    padding: 15px;
    margin: 10px auto;
    max-width: 700px;
    border-radius: 8px;
  }
</style>
</head>
<body>
<header>
  <h1>موقع الاقتباسات الملهمة</h1>
</header>
<main>
  <div id="quote-box">اضغط على الزر لتحصل على اقتباس ملهم</div>
  <div style="text-align:center;">
    <button onclick="newQuote()">اقتباس جديد</button>
  </div>

  <div id="ad-space">
    إعلان  
    <br />
    (هنا توضع إعلانات Google Adsense أو إعلانات أخرى)
  </div>
</main>
<footer>
  &copy; 2025 موقع الاقتباسات الملهمة. جميع الحقوق محفوظة.
</footer>

<script>
  const quotes = [
    "النجاح هو الانتقال من فشل إلى فشل دون أن تفقد حماسك. – وينستون تشرشل",
    "لا تنتظر الفرصة بل اصنعها. – جورج برنارد شو",
    "الحياة إما مغامرة جريئة أو لا شيء. – هيلين كيلر",
    "الإبداع هو الذكاء وهو يستمتع. – ألبرت أينشتاين",
    "الأشياء العظيمة لا تأتي من مناطق الراحة.",
    "لا تحكم على كل يوم من خلال الحصاد الذي تحصده، بل من خلال البذور التي تزرعها.",
    "المستقبل ينتمي لأولئك الذين يؤمنون بجمال أحلامهم. – إلينور روزفلت",
    "كن التغيير الذي تريد أن تراه في العالم. – مهاتما غاندي"
  ];

  function newQuote() {
    const randomIndex = Math.floor(Math.random() * quotes.length);
    document.getElementById('quote-box').textContent = quotes[randomIndex];
  }
</script>
</body>
</html>
