  <!DOCTYPE html>
<html lang="tr">

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
                                               
 
