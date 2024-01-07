<!DOCTYPE html>
<html>
<head>
  <title>我的自我介紹</title>
  <link rel="stylesheet" href="styles.css">

</head>
<body>

  <div class="background-image"></div>

  <h1>自我介紹</h1>

  <h2>你好，我是[陳廷恩]</h2>



  <label for="sectionSelect">選擇部分：</label>
  <select id="sectionSelect" onchange="showSection()">
    <option value="aboutMe">關於我</option>
    <option value="portfolio">作品</option>
  </select>

  <div id="aboutMe" style="display: none;">
      <H1>關於我<H1> 
 <h2>興趣</h2>
    <ul>
    <li>打籃球</li>
    <li>聽音樂</li>
    <li>打電動</li>
    <li>看電影</li>
    <li>畫畫</li>
  </ul>
 
  <h2>聯絡我</h2>
  <p>你可以通過郵件與我聯繫：c111181109@NKUST.EDU.TW</p>

  </div>

  <div id="portfolio" style="display: none;">
    
        <h3>我的作品</h3>
        <img src="作品.jpg" alt="作品圖片" style="width: 300px; height: auto;"></n>
        <img src="喬魯諾.jpg" alt="作品圖片" style="width: 300px; height: auto;"></n>
        <img src="煩雜.jpg" alt="作品圖片" style="width: 300px; height: auto;"></n>
        <img src="貓咪.jpg" alt="作品圖片" style="width: 300px; height: auto;"></n>
      </div>
      

  </div>

  <script>
    function showSection() {
      var sectionSelect = document.getElementById("sectionSelect");
      var aboutMe = document.getElementById("aboutMe");
      var portfolio = document.getElementById("portfolio");

      if (sectionSelect.value === "aboutMe") {
        aboutMe.style.display = "block";
        portfolio.style.display = "none";
      } else if (sectionSelect.value === "portfolio") {
        aboutMe.style.display = "none";
        portfolio.style.display = "block";
      }
    }
  </script>

</body>
</html>


  
