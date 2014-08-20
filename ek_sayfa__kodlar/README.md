# Ek Sayfa ( Kodlar )
**HTML kodları: **

     <html>
       <head><title>Baska Bir CSS</title>
        <link href="bbcss.css" type="text/css" rel="stylesheet"/>
     </head>
    <body>
     <header class="arkaplan">
       <fieldset>
          <a href="http://www.logomatik.net/image.png?fsize=30&font=A+Damn+Mess.ttf&text=web%20tasar%C4%B1m&mirror=yes&color=333300&vcolor=&bgcolor=&alpha=Yes&output=png&spacing=5&shadow=yes&transparent=yes&icon=no&iconic=&top_spacing=5&left_spacing=6&icon_size=48"/> <img class="baslik" src="http://www.logomatik.net/image.png?fsize=30&font=A+Damn+Mess.ttf&text=web%20tasar%C4%B1m&mirror=yes&color=333300&vcolor=&bgcolor=&alpha=Yes&output=png&spacing=5&shadow=yes&transparent=yes&icon=no&iconic=&top_spacing=5&left_spacing=6&icon_size=48"/> </a>
          <a class="sosyalağ1" href="http://www.facebook.com" target=new><img src="http://in.sitekodlari.com/fb/facebook4.png" border="0"></a>
          <a class="sosyalağ3" href="http://Instagram.com/" target=new><img src="http://in.sitekodlari.com/insta/8.png" border="0"></a>
          <label class="arama"><button class="change-color" type=submit>ARA</button></label>
          <input class="arama" type="search" name="googlesearch"/>
          <form class="form">
             <label> E-posta: </label> <br/>
              <input class="change-color" type="e-mail" name="user_name"/><br/>
              <label> Parola: </label><br/>
              <input class="change-color" type="controls" name="user_password"/><br>
              <input class="change-color" type="submit" name="sing-in" value="Giris yap"/>
              <input type="checkbox" name="control" value="sifre"/> <label> Beni Unutma!</label>
          </form>
       </fieldset>
     </header>
     <nav class="ikinci">
       <fieldset>
            <ul class="liste">
                <li> <a class="pozisyon" href="#" target=new>HTML</a></li>
                <li> <a class="pozisyoniki" href="#" target=new>CSS</a></li>
                <li> <a class="pozisyonuc" href="#" target=new>JavaScript</a></li>
            </ul>
       </fieldset>
     </nav>
       <fieldset>
     <div>
         <p class="mavi"><a href="#"/>Bugune padding ve margin ile hucre ici ve hucre disi bosluk verme konulariyla divlere konum belirliyordum. <br/>Px degerini ayarlamak cok zahmetli bir istir. Bugun bunun yerine CSS de konumlandirma konusunu ogrendim ve bu komutlarla sayfa ici divlerin konumlarini belirleyecegim..</a></p>

         <p class="yesil">CSS'te konumlandirma belki de CSS'in en onemli konusudur. Eger bu konuyu tam anlamiyla ogrenirseniz CSS'in yuzde ellisini ogrenmis sayilirsiniz. Bu dersimizde static, relative, absolute ve fixed gibi position degerlerini gorecegiz.<br/> Position'a yardimci olan float ve clear ozelliklerini de ogrenecegiz.</p>                                                                                                 </a> <p class="kirmizi"><a href="#">Bu bir css çalışmasıdır. CSS çalışarak kendimi geliştireceğim ve bu çalışmalarımla web tabanlı programlamaya adım atıyorum.</br> kız arkadaşımla da dertlerim bitmiyo hiçbişeyin normal gittiği yok niye böyle valla bende bilmiyorum.</a></p>

		 <aside class="yankenar">
     <script language="javascript" src="http://in.sitekodlari.com/takvim3.js"></script>
       <script language="javascript" src="http://in.sitekodlari.com/tarih.js"></script>
     <ul class="kategori">
     <li><a href="sayfalinki">Ana Kategori 1</a>
        <ul>
            <li><a href="altkategorilinki">Alt Kategori1</a></li>
            <li><a href="altkategorilinki">Alt Kategori2</a></li>
            <li><a href="altkategorilinki">Alt Kategori3</a></li>
        </ul>
      </li>
     <li><a href="sayfalinki">Ana Kategori 2</a>
        <ul>
            <li><a href="altkategorilinki">Kategori 2 alt kategori</a></li>
        </ul>
    </li>
    <li><a href="sayfalinki">Ana Kategori 3</a>
        <ul>
            <li><a href="altkategorilinki">kategori3 alt kategorisi</a></li>
        </ul>
    </li>
    <li><a href="sayfalinki">Ana Kategori 4</a>
        <ul>
            <li><a href="altkategorilinki">kaetgori4 alt kategorisi</a></li>
        </ul>
      </li>
     </ul>
     </aside>
        </div>
      </fieldset>
     </body>
    </html>
**CSS kodları:**

     div {font-family: Verdana, monospace,      sans-serif;font-weight:   bold;padding:0px;margin:50px;	  background-repeat:no-repeat;position:relative;top:-75px;right:-150px;	}
    .mavi {width: 300px;background-color: skyblue;padding: 20px;margin-top: 15px;border-style:solid;font-size:12px;text-align:justify;	margin-left:500px;margin-top:-15px;box-shadow: 10px 10px 5px #888888;position:relative;top:50px;text-decoration:none;}
    .yesil {width: 300px;background-color: lightgreen;padding: 20px; margin-top: 15px;border:solid;border-radius:150px;font-size:12px;text-align:justify;	margin-top:-150px;margin-left:20px;box-shadow: 10px 10px 5px #888888;position:relative;top:50px;left:50px;}
    .kirmizi {width: 300px;background-color: lightcoral;padding: 20px;margin-top: 15px;border:solid 2px;border-radius:200px 150px / 250px 10px;font-size:10px;text-align:justify;padding:40px;margin-top:150px;box-shadow: 10px 10px 5px #888888;position:relative;bottom:50px;left:100px;}
    .liste li {display:inline;}
    a{text-decoration:none;text-shadow:1px 2px 5px blue;}
    .ikinci{text-align:center;position:relative;top:-40px;margin-top:50px; }
    .baslik{width:300; height:120;background-color:;}
    body{
    background: rgb(254,191,1); /* Old browsers */
    background: -moz-linear-gradient(top,  rgba(254,191,1,1) 0%, rgba(254,191,1,1) 15%, rgba(254,191,1,1) 33%, rgba(254,191,1,1) 33%, rgba(254,191,1,1) 42%, rgba(254,191,1,1) 56%, rgba(254,191,1,1) 60%, rgba(254,191,1,1) 73%, rgba(254,191,1,1) 76%, rgba(254,191,1,1) 97%); /* FF3.6+ */
    background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,rgba(254,191,1,1)), color-stop(15%,rgba(254,191,1,1)), color-stop(33%,rgba(254,191,1,1)), color-stop(33%,rgba(254,191,1,1)), color-stop(42%,rgba(254,191,1,1)), color-stop(56%,rgba(254,191,1,1)), color-stop(60%,rgba(254,191,1,1)), color-stop(73%,rgba(254,191,1,1)), color-stop(76%,rgba(254,191,1,1)), color-stop(97%,rgba(254,191,1,1))); /* Chrome,Safari4+ */
    background: -webkit-linear-gradient(top,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* Chrome10+,Safari5.1+ */
    background: -o-linear-gradient(top,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* Opera 11.10+ */
    background: -ms-linear-gradient(top,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* IE10+ */
    background: linear-gradient(to bottom,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* W3C */
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#febf01', endColorstr='#febf01',GradientType=0 ); /* IE6-9 */
     }
      .pozisyon{position:relative;left:-50px;font-size:30px;}
    .pozisyoniki{position:relative;left:-5px;font-size:30px;}
    .pozisyonuc{position:relative;right:-30px;font-size:30px;}
     .form{position:absolute;right:15px;top:20px;}
    .arkaplan{background-color:;}
    .yankenar{width:200px;position:relative;top:-400px;left:-200px}
    .arama{position:relative;left:125px;width:400px;font-size:20px;font-style:italic;text-decoration:bold;font-weight:bold;}
     .sosyalağ1{position:absolute;top:30px;right:750px;}
    .sosyalağ2{position:absolute;top:30px;right:650px;}
    .sosyalağ3{position:absolute;top:20px;right:550px;}
    button{font:17px bold;}
    .change-color:hover{background-color:skyblue;}
    .kategori { margin:0; padding:0; list-style:none; position:relative; top:20px; }
    .kategori li a { display:block; padding:3px; margin:0px; color:#000; position:relative; top:20px;}
    .kategori li ul { display:none; margin:0px; padding:0px; list-style:none;position:relative; top:20px; }
    .kategori li ul a { color:#555;position:relative; top:20px;}

