<!DOCTYPE html>
<html>
<meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/>
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@400;700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Sono:wght@600&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Nerko+One&display=swap" rel="stylesheet">

  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script>
  <script src="https://unpkg.com/typeit@8.7.0/dist/index.umd.js"></script><link href="https://feeldreams.github.io/forkamuaja/style.css" rel="stylesheet" type="text/css" />
  <script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script>
  
<head>
<title>Pantun Romantis Buat Kamu</title>
<link rel="icon" type="image/x-icon" href="https://malasid.github.io/favicon.png">
<meta name="description" content="HTML Replit Coding">
<!-- 
  Made with love by Rayys!
  
     Blog: feeldream.id
     Instagram: @rayyarrr
     TikTok: @feelthisray
     Email: rayyarr73@gmail.com
     
  Thanks to all <3
-->
</head>
<body>
  
   <!-- Ganti Audio di sini -->
   <audio src="https://feeldreams.github.io/angelbabypart2.mp3" id="linkmp3" class="sembunyi"></audio>
   
   <div id="bodyblur">
     <!-- Wallpaper --><img src="https://feeldreams.github.io/pics/awan1.jpg" id="wallpaper"/>
   </div>
   
   <div id='Content'>

     <div id="ftAwal">
       <!-- Stiker Pembuka -->
       <img src="https://feeldreams.github.io/pandaputih.gif" id="ftoAwal"/>
     </div>

     <div id="loveIn">
       <!-- Tombol LOVE --><label class='lovein'>❤️</label>
     </div>
     <p id="ket">Sentuh LOVEnya!</p>
     
     <div class="kumpulanstiker">
         <!-- Stiker untuk Konten -->
         <img src="https://feeldreams.github.io/bunga.gif" id="fotostiker"/>
         <img src="https://feeldreams.github.io/emawh.gif" id="fotostiker1"/>
         <img src="https://feeldreams.github.io/pandakuning.gif" id="fotostiker2"/>
         <img src="https://feeldreams.github.io/pusn.gif" id="fotostiker3"/>
         <img src="https://feeldreams.github.io/gumush.gif" id="fotostikerA"/>
     </div>
     
     <div><div id='pergeseran'>
      
        <p><b>
          <span>hai kamuuu<br>aku ada pantun buat kamu</span>
        </b></p>
        
        <p><b>
          <span>ikan hiu bawa koper</span>
        </b></p>
        
        <p><b>
          <span>i love uu forever<3333</span>
        </b></p>

        <p><b>
          <span>sate² apa yg bikin aku bahagia?</span>
        </b></p>

        <p><b>
          <span>saterusnya sama kamu<br>😍😆🥰🤭🤣</span>
        </b></p>
        
        <p><b>
          <span id="iniakhir">terakhir nihh ><</span>
        </b></p>
       
     </div></div>

     <p id="ketgeser">Klik untuk Geser!</p>

     <div><blockquote id='bq'>
       <p id="kalimat"></p>
       <p id="pesanAkhir" class="gaya4"></p>
     </blockquote></div>

   </div>
   
<script>
  const body = document.querySelector("body");const swalst = Swal.mixin({timer: 2500, allowOutsideClick: false, showConfirmButton: false, timerProgressBar: true, imageHeight: 90,}); audio = new Audio('' + linkmp3.src); ftganti=0;fungsi=0;fungsiAwal=0;deffotostiker=fotostiker.src;function berjatuhan() {const heart = document.createElement("div"); heart.className = "fas fa-heart"; heart.style.left = (Math.random() * 90)+"vw"; heart.style.animationDuration = (Math.random()*3)+2+"s"; body.appendChild(heart);} setInterval(function name(params) {var heartArr = document.querySelectorAll(".fa-heart"); if (heartArr.length > 100) {heartArr[0].remove()}},100);Content.style = "opacity:1;margin-top:14vh"; const swals = Swal.mixin({allowOutsideClick: false, cancelButtonColor: '#FF0040', imageHeight: 80,}); 
  
  teksAkhir = "di jalan ada lampu,<br>di kuburan ada hantu,<br>di kerajaan ada ratu,<br>tapi di hatiku...<br>cuma ada kamu, jiakhhh<3333";
  teksAkhirB = "i love uuu ><";
  document.getElementById("loveIn").onclick = function() {
    if(fungsiAwal==0){
      audio.play();
      loveIn.style="transition:all .8s ease;transform:scale(15);opacity:0";
      ftAwal.style="opacity:0";
      wallpaper.style="transform: scale(1);";
      ket.style="display:none";
      fungsiAwal=1;setTimeout(initengahan,300);setTimeout(pgmuncul,600)
    }
  }
  
  const box = document.getElementById('pergeseran');
  const directChildren = box.children.length;
  console.log('Script ini dibuat oleh: www.feeldream.id');
  console.log('Instagram: @rayyarrr');
  console.log('Total Slide: ', directChildren);
  totalPesan = directChildren;
  
  aktigeser=0;thisgeser=1;
  document.getElementById("bodyblur").onclick = function() {
    if(aktigeser==1){
      document.getElementById('pergeseran').scrollLeft += 300;
      hsementara();
      if(thisgeser>1){
      if(thisgeser%2==0){wallpaper.style="transform: scale(2)";} else {wallpaper.style="transform: scale(1)";}
      }
      if(thisgeser==3){
        ftganti=1;fthilang();
      }
      if(thisgeser==4){
        ftganti=0;fthilang();
      }
      if(thisgeser==5){
        ftganti=2;fthilang();
      }
      if(thisgeser==6){
        ftganti=3;fthilang();
      }
    }
  }
  function hsementara(){
    ketgeser.style="position:relative;";
    thisgeser+=1;aktigeser=0;setTimeout(munculkembali,500)
  }
  function munculkembali(){
    if(thisgeser<totalPesan){
      ketgeser.style="position:relative;transform:scale(1);opacity:.8";
      aktigeser=1;
    }
    if(thisgeser==totalPesan){setTimeout(aksiakhir,900)}
  }
  
  function aksiakhir(){
    ketgeser.style="";
    ftganti=9;ftmuncul();
    pergeseran.style="position:relative;margin-top:5vh;transform:scale(0);";
    iniakhir.style="opacity:0";setTimeout(bqmuncul,400);
  }
  
  kalimat.innerHMTL="";
  function kalimatakhir(){
    iniakhir.style="";iniakhir.innerHTML="";
    new TypeIt("#kalimat", {
      strings: ["" + teksAkhir],
      startDelay: 50, speed: 50, cursor: true,
      afterComplete: function(){
         setTimeout(mulaiketikA,300);
         kalimat.innerHTML=teksAkhir;
      },}).go();
  }
  
  function initengahan(){
    ftAwal.style="display:none";loveIn.style="display:none";ket.style="display:none";
    Content.style = "opacity:1;margin-top:7vh";
  }
  
  function ftmuncul(){
    if(ftganti==0){fotostiker.src = deffotostiker;}
    if(ftganti==1){fotostiker.src = fotostiker1.src;}
    if(ftganti==2){fotostiker.src = fotostiker2.src;}
    if(ftganti==3){fotostiker.src = fotostiker3.src;}
    
    if(ftganti!=1 && ftganti!=9 && ftganti!=10){fotostiker.style="display:inline-flex;opacity:1;transform:scale(1)";}
    if(ftganti==11){fotostiker.src = fotostikerA2.src;}
    
    if(ftganti==1 || ftganti==2){fotostiker.style="display:inline-flex;opacity:1;transform:scale(1);width:120px;height:120px;padding:none;background:none;box-shadow:none;border-radius:0;border:none";}
    if(ftganti==9){fotostiker.style="display:inline-flex;opacity:0;transform:scale(1);padding:none;background:none;box-shadow:none;border-radius:0;border:none";}
    if(ftganti==10){fotostiker.src = fotostikerA.src;fotostiker.style="display:inline-flex;opacity:1;transform:scale(1);width:120px;height:120px;padding:none;background:none;box-shadow:none;border:none;border-radius:0;";}
  }
  function fthilang(){fotostiker.style="display:inline-flex;opacity:0;transform:scale(0)";if(ftganti<=11){setTimeout(ftmuncul,250)} if(ftganti>=12){wallpaper.style="opacity:.7;transform: scale(2);";}}
  function jjfoto(){fotostiker.style.animation="rto .8s infinite alternate";}
  
  function pgmuncul(){pergeseran.style="position:relative;margin-top:5vh;opacity:1;visibility:visible;transform:scale(1);";ftmuncul();setTimeout(munculkembali,500)}
  function bqmuncul(){pergeseran.style="display:none";bq.style = "position:relative;opacity:1;visibility:visible;margin-top:0;transform: scale(1);";setTimeout(kalimatakhir,200);}
  function bqhilang(){wallpaper.style="transform: scale(2);";bodyblur.style="opacity:.3";bq.style = "position:relative;transition:all .7s ease;";}
  
  function tombol(){Tombol.style="opacity:1;transform: scale(1);";}
  
  pesanAkhir.innerHTML = "";
  function mulaiketikA(){
  ftganti=10;ftmuncul();setInterval(berjatuhan,250);
  pesanAkhir.style="position:relative;opacity:1;visibility:visible;transform: scale(1)";
  new TypeIt("#pesanAkhir", {
  strings: ["" + teksAkhirB], startDelay: 100, speed: 50, cursor: false, deleteSpeed: 20, breakLines: false, waitUntilVisible: true, lifelike: true,
  afterComplete: function(){
      pesanAkhir.style.animation="rto .8s infinite alternate";
  },}).go();
  }
</script>
<script >
  
</script>
</body>
</html>
