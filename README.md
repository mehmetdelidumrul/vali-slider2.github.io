  <!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vali Ünal Erkan İlkokulu Slider</title>

  <!-- Basit stiller -->
  <style>
    body {
      margin: 0;
      background-color: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .slider {
      position: relative;
      width: 100%;
      max-width: 600px;
      overflow: hidden;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.3);
    }
    .slides {
      display: flex;
      transition: transform 0.8s ease;
    }
    .slide {
      min-width: 100%;
      box-sizing: border-box;
    }
    img {
      width: 100%;
      height: auto;
      display: block;
    }
  </style>
</head>
<body>

  <div class="slider">
    <div class="slides" id="slides">
      <div class="slide"><img src="https://valiunalerkani.meb.k12.tr/meb_iys_dosyalar/61/01/710204/resimler/2023_12/22_111514_1.jpg" alt=""></div>
      <div class="slide"><img src="https://valiunalerkani.meb.k12.tr/meb_iys_dosyalar/61/01/710204/resimler/2023_12/22_111523_2.jpg" alt=""></div>
      <div class="slide"><img src="https://valiunalerkani.meb.k12.tr/meb_iys_dosyalar/61/01/710204/resimler/2023_12/22_111531_3.jpg" alt=""></div>
    </div>
  </div>

  <script>
    let index = 0;
    const slides = document.getElementById("slides");
    const total = slides.children.length;

    setInterval(() => {
      index = (index + 1) % total;
      slides.style.transform = `translateX(-${index * 100}%)`;
    }, 3000);
  </script>

</body>
</html>
                                               
 
