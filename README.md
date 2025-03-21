# Bang-BiL

<!DOCTYPE html>
<html>
<meta charset='UTF-8'/>
<meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/>
<meta content='IE=edge' http-equiv='X-UA-Compatible'/>
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@400;700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Caveat&display=swap" rel="stylesheet">

  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><script src="https://hbdkamu.feeldream.repl.co/script.js"></script>
  <script src="https://unpkg.com/typeit@8.7.0/dist/index.umd.js"></script>
  <script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script>
  
<head>
<title>Script HTML buat Kamu</title>
<meta name="description" content="HTML Feeldream Repl Co">
<!-- 
  Made with love by Rayys!
  
     Blog: feeldream.id
     Instagram: @rayyarrr
     TikTok: @feelthisray
     Email: rayyar73@gmail.com
     
  Thanks to all <3
-->
</head>
<style>
:root {
--warna-bg: rgba(0, 0, 0, .3); 
--tombol-teks: #fff;
--tombol-bingkai: #fff;
--bingkai: 18px;
--bingkai-kiri: 1.3px solid var(--tombol-bingkai);
--bingkai-kanan: 1.3px solid var(--tombol-bingkai);
--gaya-font: 'Nunito Sans', sans-serif;
--gaya-font2: 'Caveat', cursive;
}
@keyframes fanim {0% {background-position: 0% 0%;}25% {background-position: 100% 100%;} 50% {background-position: 0% 100%;} 75% {background-position: 50% 50%;} 100% {background-position: 0% 0%;}}
body{background-color:#000;font-family:var(--gaya-font);padding: 20px 25px;-webkit-user-select: none; -ms-user-select: none; user-select: none;} a{text-decoration:none;}
body::before{content:"\00A9  Rayys | feeldream.id";color:white;opacity:.3;font-size:10px;position:fixed;bottom:25px;right:25px;z-index:2}
#bodyblur{animation: jj 7s infinite;opacity:.5;position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,.3);transition:all 1s ease;} 
#wallpaper{width:100%;height:100%;transform: scale(1);transition:all 1.7s ease;}
#beneranblur{position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,.3);transition:all 3s ease;}

@keyframes jj{0%  {transform: scale(1);} 50% {transform: scale(1.3);} 100% {transform: scale(1);}}
@keyframes rts{from {transform:scale(.1);} to {transform:scale(1);}}
@keyframes rto{from {transform:scale(1);} to {transform:scale(1.1);}}
@keyframes aniopa{0% {transform: scale(1);} 50% {transform: scale(.75);} 100% {transform: scale(1);}}
@keyframes rtf{from {transform: rotate(0deg);} to {transform: rotate(360deg);}} @keyframes rt{from {transform: scale(.9);/* transform: rotate(-5deg); */} to {transform: scale(1);/* transform: rotate(5deg); */}}
@keyframes kont{0%  {left:-1px; top:-3px;} 50% {left:1px; top:3px;} 100% {left:-1px; top:-3px;}}

blockquote{position:absolute;opacity:0;visibility:hidden;/*background:var(--warna-bg);border: 1px solid rgba(255, 255, 255, 0.5);border-radius:var(--bingkai);box-shadow: rgba(255,255,255, 0.3) 0px 7px 29px 0px;*/transform: scale(.1);transition:all .7s ease;margin-left:0;margin-right:0;color:var(--tombol-teks);text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);/*backdrop-filter:blur(2px);*/}
blockquote{width:400px;text-align:center;line-height:1.3em;padding:0}
blockquote p{font-size:15px;font-weight:400;line-height:1.5em;transition:all .5s ease;margin-left:0;margin-right:0}
blockquote p:not(#kalimat, #teksnim){display:none;}
#teksnim, blockquote p span.ft{font-family:var(--gaya-font2);font-size:20px;font-weight:700}
#teksnim{font-size:22px;position:absolute;opacity:0;transform:scale(0);transition:all .8s ease}

#pergeseran{margin-top:40px;position:absolute;opacity:0;transform:scale(0);transition:all 1s ease;display:flex;flex-wrap:nowrap;align-items:flex-start;justify-content:flex-start;max-width:500px;padding:0 30px; overflow-y:hidden;overflow-x:hidden;scroll-behavior:smooth;scroll-snap-type:x mandatory; -ms-overflow-style:none;-webkit-overflow-scrolling:touch}
#pergeseran p{background:rgba(0, 0, 0, .5);border-left:2px solid #fff;border-right:2px solid #fff; padding:15px;display:flex;flex-wrap:nowrap;text-align:center;line-height:1.4em;align-items:center;justify-content:center;flex-shrink:0; width:90%;margin:0 15px 0 0; scroll-snap-align:center}
#pergeseran p, #psn{color:white;text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);min-height:150px;}
#pergeseran > *:last-child{margin-right:0} #pergeseran:after{content:'';display:block;flex-shrink:0; align-self:stretch;padding-left:20px}
#pergeseran p b{display:block;}
#pergeseran p b span{font-size:15px;font-weight:700;}
#pergeseran p b span.ft{font-family:var(--gaya-font2);font-size:20px}
#pergeseran p b img{width:80px;height:80px;margin-bottom:20px;}
#fotolove{border-radius:50%;transition:all .3s ease;} #fotolove:hover{transform: scale(.8);}
#pesanAkhir{margin-top:30px;font-family:var(--gaya-font3);font-size:22px !important;font-weight:400;text-align:center;position: absolute;opacity:0;}

#Tombol{position:relative;opacity:0;margin-top:20px !important;display:flex;align-items:left;list-style:none;transform: scale(.1);transition:all .7s ease;}
#Tombol a{cursor:pointer;display:inline-flex;align-items:center; margin:0;margin:12px 0 12px 0;transition:all .2s ease;padding:10px;outline:0;border-left:2px solid #fff;border-right:2px solid #fff; border-radius:0;line-height:15px;background:rgba(0,0,0,.5);color:white;font-size:12px;font-weight:400;white-space:nowrap;overflow:hidden;z-index:1} 
#Tombol a:hover{transform: scale(.90);opacity:.98;}

#Content{animation-name:none;animation-duration: 3s;animation-iteration-count: infinite;position:relative;opacity:0;margin-top:50px;width:100%;height:180px;transition:all .7s ease;}
#Content > *{display:flex;align-items:center;text-align:center;justify-content:center;margin-top:1px;}
.kumpulanstiker > img{display:none;background:rgba(255,255,255, .5);box-shadow: 0 4px 30px rgba(255,255,255, 0.2);backdrop-filter: blur(5px);-webkit-backdrop-filter: blur(5px);border: 1px solid rgba(255, 255, 255, 1);border-radius: 50%;padding:10px;width:92px;height:92px;}
#ftAwal > img{width:130px;height:130px;margin-bottom:50px;}
#fotostiker{opacity:.1;transition:all .7s ease;transform: scale(.1);}
#imglewat{margin:30px 0;opacity:0;max-width:520px;height:100px;position:absolute;transition:all 1s ease;}

.halo{text-align:center;font-size:17px !important;position:relative;margin-bottom:20px} 
.halo.gaya2{font-family:var(--gaya-font2);font-size:24px !important;margin-top:20px !important;}
.halo.sty3{position:absolute !important;font-size:14px !important;font-weight:400 !important;margin:30px 20px !important;}

#fotolove img{transition:all .5s ease;width:75px;height:75px;padding:0;background:none}
#loveIn img{display:inline-flex;background:none;width:130px;height:130px;transition:all .3s ease;} 
#ket, #ketgeser, .halo{text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);font-size:17px;font-weight:700;color:white}
#ket{margin-top:20px !important;font-size:12px;font-weight:400;opacity:.8}
#ketgeser{position:absolute;margin-top:30px;font-size:10px;font-weight:400;transform:scale(0);opacity:0;transition:all .7s ease;}

@keyframes leaves {0% {transform: scale(1.0);} 100% {transform: scale(.85);}}
#loveIn{animation: leaves .7s ease-in-out infinite alternate;-webkit-animation: leaves 1s ease-in-out infinite alternate;} 
.lovein{background:#fff;border-radius:50%;width:40px;height:40px;padding:10px;font-size:30px;display:flex;align-items:center;text-align:center;justify-content:center;transition:all .3s ease;}
.lovein:hover{cursor:pointer}
.lovein svg{stroke:#ff0000;stroke-width:1.3;fill:none;width:35px;height:35px}

.swal2-modal > *{font-family:var(--gaya-font);font-size:16px;color:white}
.swal2-title{line-height:1.3em;font-size:17px;text-align:center;padding:15px 30px 0 30px;}
.swal2-timer-progress-bar-container > *{opacity:.7;background:#00B6FF;margin:0 2px}
.swal2-modal{background: rgba(0,0,0, .6);backdrop-filter: blur(3px);-webkit-backdrop-filter: blur(3px);box-shadow: 0 4px 30px rgba(255,255,255, 0.3);border: 1px solid rgba(255, 255, 255, 0.3);border-radius: 14px;max-width:280px;top:-60px;}
.swal2-image{background: rgba(255, 255, 255, 0.5);box-shadow: 0 4px 30px rgba(255,255,255, 0.3);backdrop-filter: blur(5px);-webkit-backdrop-filter: blur(5px);border: 1px solid rgba(255, 255, 255, 0.3);border-radius: 50%;padding:10px;}
.swal2-styled.swal2-confirm, .swal2-styled.swal2-cancel{position: relative;background-color: #4839eb;color: #fff;font-size:14px;border:1px solid #ffffff59;border-radius:4px;z-index: 1;transition: all 0.2s;}

.fa-heart {opacity:.3;color:white;font-size: 20px;position: absolute;animation:  heartMove linear 1;top: -10vh;z-index: 0;}
@keyframes heartMove {0%{transform: translateY(-10vh) ;} 100%{transform: translateY(100vh) ;}}
.sembunyi, #pesanditolak > *, #kado2, #kado3, .kumpulanwp > *{display:none !important}
</style>
<body>
	
   <!-- Ganti Audio di sini -->
   <audio src="https://feeldreams.github.io/audio/anditsnot.mp3" id="linkmp3" class="sembunyi"></audio>
   
   <div id="bodyblur">
     <!-- Wallpaper / Background --><img src="https://feeldreams.github.io/pics/awan3.jpg" id="wallpaper"/>
   </div>
   
   <div id='Content'>

     <div id="ftAwal">
       <!-- Stiker Pembuka -->
       <img src="https://feeldreams.github.io/pandaputih.gif" id="ftoAwal"/>
     </div>

     <div id="loveIn">
       <!-- Tombol LOVE -->
       <a href="https://www.feeldream.id/2023/01/script-feeldream.html?m=1#hbd" target="_blank" class='lovein'><svg class='line' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'><g transform='translate(2.550170, 3.550158)'><path d='M0.371729633,8.89614246 C-0.701270367,5.54614246 0.553729633,1.38114246 4.07072963,0.249142462 C5.92072963,-0.347857538 8.20372963,0.150142462 9.50072963,1.93914246 C10.7237296,0.0841424625 13.0727296,-0.343857538 14.9207296,0.249142462 C18.4367296,1.38114246 19.6987296,5.54614246 18.6267296,8.89614246 C16.9567296,14.2061425 11.1297296,16.9721425 9.50072963,16.9721425 C7.87272963,16.9721425 2.09772963,14.2681425 0.371729633,8.89614246 Z'></path><path d='M13.23843,4.013842 C14.44543,4.137842 15.20043,5.094842 15.15543,6.435842'></path></g></svg></a>
     </div>
     <p id="ket">Sentuh LOVEnya!</p>

     <div class="kumpulanstiker">
         <!-- Stiker untuk Konten -->
         <img src="https://feeldreams.github.io/cilukba.gif" id="fotostiker"/>
         <img src="https://feeldreams.github.io/pandaputih.gif" id="fotostikerPopup"/>
         <img src="https://feeldreams.github.io/weee.gif" id="fotostikerPopupCon"/>
         <img src="https://feeldreams.github.io/ngumpet.gif" id="fotostikerPopupCan"/>
     </div>
     
     <div><div id='pergeseran'>
     	
<!-- Pesan -->
<p><b><img src="https://feeldreams.github.io/g5.gif"/><br>
	<span>Hai Afifah 🤭❤️</span>
</b></p>

<p><b><img src="https://feeldreams.github.io/pusn.gif"/><br>
	<span>Aku Cuma Mau<br>Bilang Nih 😆</span>
</b></p>

<p><b><img src="https://feeldreams.github.io/cilukba.gif"/><br>
	<span>Ciyee yang Hari Ini Ultah 😜</span>
</b></p>

<p><b><img src="https://feeldreams.github.io/g5.gif"/><br>
	<span class="ft">Selamat Ulang Tahun! 🥳</span>
</b></p>

<p><b><img src="https://feeldreams.github.io/mndkat.gif"/><br>
	<span>Panjang Umur dan<br>Sehat Selalu yaa 🥰</span>
</b></p>

     </div></div>
     
     <!-- Edit Pesan Akhir di Sini -->
     <div><blockquote id='bq'>
       <p id="teksnim">Happy Level Up Day! 🥳</p>
       <p id="kalimat"><span id="klganti">Canda yaa wkwk 🤣<br><br></span>Intinya semoga di hari bertambahnya<br>usia kamu ini, kamu bisa menjadi<br>pribadi yang lebih baik lagi yaa..<br>semoga kamu makin dewasa, makin cantik, makin imut dan lucu🥰<br><br><span class="ft">Wish You All The Best ✨</span></p>
     </blockquote></div>
     
     <!--<p id="ketgeser">Klik untuk Geser!</p>-->
     <div id="Tombol">
       <a onClick="multifungsi()">
         <b id="tmbl">Geser &#128073;</b>
       </a>
     </div>
     
   </div>

<script>
const body = document.querySelector("body"); const iniwp = [];iden = 1; const swals = Swal.mixin({timer: 99999, allowOutsideClick: false, showConfirmButton: true, timerProgressBar: false, imageHeight: 90,}); audio = new Audio('' + linkmp3.src); ftganti=0;fungsi=0;fungsiAwal=0;deffotostiker=fotostiker.src;
function berjatuhan() {const heart = document.createElement("div"); heart.className = "fas fa-heart"; heart.style.left = (Math.random() * 90)+"vw"; heart.style.animationDuration = (Math.random()*3)+2+"s"; body.appendChild(heart);} setInterval(function name(params) {var heartArr = document.querySelectorAll(".fa-heart"); if (heartArr.length > 100) {heartArr[0].remove()}},100);Content.style = "opacity:1;margin-top:14vh"; 

const box = document.getElementById('pergeseran');
const totalSlide = box.children.length;
console.log('Total Slide: ', totalSlide);
totalPesan = totalSlide;

var date = new Date();
var days = ["Minggu", "Senin", "Selasa", "Rabu", "Kamis", "Jumat", "Sabtu"];
var months = ["Januari", "Februari", "Maret", "April", "Mei", "Juni", "Juli", "Agustus", "September", "Oktober", "November", "Desember"];
var hours = date.getHours();
var minutes = date.getMinutes();

// Tambahkan awalan nol jika jam atau menit kurang dari 10
if (hours < 10) {hours = "0" + hours;}
if (minutes < 10) {minutes = "0" + minutes;}

var day = days[date.getDay()];
var dateNum = date.getDate();
var month = months[date.getMonth()];
var year = date.getFullYear();

console.log(hours + "." + minutes + " WIB - " + day + ", " + dateNum + " " + month + " " + year);
// Dapatkan elemen yang ingin ditambahkan watermark
var element = document.getElementById("Content");

// Buat elemen baru untuk menampung watermark
var watermark = document.createElement("div");

// Setel teks watermark dan propertinya
watermark.textContent = day + ", " + dateNum + " " + month + " " + year;
watermark.style = "color:white;opacity:.5;font-size:10px;position:fixed;bottom:25px;left:25px;z-index:2";

// Tambahkan elemen watermark ke dalam elemen utama
element.appendChild(watermark);

//////////////////////////////////////////////////

  var sudahklik = false;
  sudahklik = true;
      	loveIn.innerHTML = "<label class='lovein'><svg class='line' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'><g transform='translate(2.550170, 3.550158)'><path d='M0.371729633,8.89614246 C-0.701270367,5.54614246 0.553729633,1.38114246 4.07072963,0.249142462 C5.92072963,-0.347857538 8.20372963,0.150142462 9.50072963,1.93914246 C10.7237296,0.0841424625 13.0727296,-0.343857538 14.9207296,0.249142462 C18.4367296,1.38114246 19.6987296,5.54614246 18.6267296,8.89614246 C16.9567296,14.2061425 11.1297296,16.9721425 9.50072963,16.9721425 C7.87272963,16.9721425 2.09772963,14.2681425 0.371729633,8.89614246 Z'></path><path d='M13.23843,4.013842 C14.44543,4.137842 15.20043,5.094842 15.15543,6.435842'></path></g></svg></label>";
  document.getElementById("loveIn").onclick = function() {
      if(sudahklik == true && fungsiAwal==0){
        loveIn.style="transition:all .5s ease;opacity:0";
        ftAwal.style="transition:all .5s ease;opacity:0";
        ket.style="transition:all .5s ease;opacity:0";
        fungsiAwal=1;setTimeout(initengahan,300);
      } else {
      	
      }
    }
  
  function initengahan(){
    ftAwal.style="display:none";loveIn.style="display:none";ket.style="display:none";
    Content.style = "opacity:1;margin-top:10vh";
    setTimeout(inipesan,200);audio.play();
  }
  
aktigeser=0;thisgeser=1;
document.getElementById("bodyblur").onclick = function() {multifungsi()}

function multifungsi(){
  if(aktigeser==1){
    if(thisgeser==totalPesan){aksiakhir()}
    document.getElementById('pergeseran').scrollLeft += 300;
    hsementara();
    //ftganti++;
    //fthilang();
  }
  if(thisgeser==100){Tombol.style="";setTimeout(aksibalas,150);}
}

  async function inipesan(){nama = "Kamu";window.nama = nama;mulainama();}  
  
  async function mulainama() {
    setTimeout(pgmuncul,200);
    //ftmuncul();
  }

  function hsementara(){
    //ketgeser.style="position:relative;";
    Tombol.style="";
    thisgeser+=1;aktigeser=0;setTimeout(munculkembali,500)
  }
  function munculkembali(){
    if(thisgeser<=totalPesan){
      //ketgeser.style="position:relative;transform:scale(1);opacity:.7";
      Tombol.style="opacity:1;transform: scale(1)";
      aktigeser=1;
    }
    if(thisgeser==50){tmbl.innerHTML = "💌 Balas";Tombol.style="opacity:1;transform: scale(1)";thisgeser=100;}
    //if(thisgeser==totalPesan){aksiakhir();thisgeser=50}
  }
  
  function aksiakhir(){
  	   pergeseran.style="position:relative;";
         //ketgeser.style="position:relative";
         Tombol.style="";
         setTimeout(aksibalas,500);
  }
  
  function kalimatakhir(){
  	new TypeIt("#kalimat", {
      strings: ["" + katakata], startDelay: 50, speed: 54, cursor: true,
      afterComplete: function(){
      	kalimat.innerHTML = katakata;
          setTimeout(munculteksnim,300);
          //tmbl.innerHTML = "💌 Balas";thisgeser=100;
          //Tombol.style="opacity:1;transform: scale(1)";
      },}).go();
  }
  function munculteksnim(){
    klganti.style="display:none";
    teksnim.style="position:relative;opacity:1;transform:scale(1);";
    setTimeout(jjteksnim,550);
    setInterval(berjatuhan,250);
  }
  function jjteksnim(){teksnim.style.animation="rto .8s infinite alternate";}
  
  function ftmuncul(){
    if(ftganti==0){fotostiker.src = deffotostiker;}
    if(ftganti==1){fotostiker.src = fotostiker1.src;}
    if(ftganti==2){fotostiker.src = fotostiker2.src;}
    if(ftganti==3){fotostiker.src = fotostiker3.src;}
    if(ftganti<=10){fotostiker.style="display:inline-flex;opacity:1;transform:scale(1)";}
  }
  function fthilang(){fotostiker.style="display:inline-flex;opacity:0;transform:scale(0)";if(ftganti<10){setTimeout(ftmuncul,250)}}
  function jjfoto(){fotostiker.style.animation="rto .8s infinite alternate";}
  
  function pgmuncul(){pergeseran.style="position:relative;opacity:1;transform:scale(1);";setTimeout(munculkembali,500)}
  function bqmuncul(){
    if(poinjwb==1){
      katakata = kalimat.innerHTML;kalimat.innerHTML = "";
    }else{
      klganti.innerHTML="Udah ah segitu aja 🤣<br><br>";katakata = kalimat.innerHTML;kalimat.innerHTML = "";
    }
    Content.style = "opacity:1;margin-top:8vh";fotostiker.style="display:none";pergeseran.style="display:none";Tombol.style="";bq.style = "position:relative;opacity:1;visibility:visible;margin-top:5vh;transform: scale(1);";
    setTimeout(kalimatakhir,200);ftganti=0;fthilang();
  }
  function bqhilang(){wallpaper.style="transform: scale(2);";bodyblur.style="opacity:.3";bq.style = "position:relative;transition:all .7s ease;";}
  
  tompositif = "Mau";
  tomnegatif = "Gamau";
  async function aksibalas(){
    var { isConfirmed: prtanya } = await swals.fire({
      title: nama + ' Mau Kado Gak Nih? 🤭❤️',
      imageUrl: '' + fotostikerPopup.src, showCancelButton: true, confirmButtonText: '' + tompositif, cancelButtonText: '' + tomnegatif,});
    if(prtanya){
       await swals.fire({
         title: 'Tapi Boong! 🤣', 
         html: 'aku bingung mau kasih kado apa ke kamu, takutnya km ga suka sm kado yg aku kasih<br>jadi km bilang yaa mau kado apa dari aku😜❤️', 
         imageUrl: '' + fotostikerPopupCon.src,
       });
       poinjwb=1;
    } else {
	     await swals.fire({
         title: 'Yaaahh!', 
         html: 'Yaudah kalo gamau 😜❤️', 
         imageUrl: '' + fotostikerPopupCan.src,
       });
       poinjwb=2;
    }
    bqmuncul();
    }
</script>
<!-- Sampai Sini -->
</body>
</html>
