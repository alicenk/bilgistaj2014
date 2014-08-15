#Dördüncü hafta
##4. gün
**14/08/2014**

Bu gün web sayfasında header kısmını kodlamayı divlerle işlem yapmayı ve divleri, elementleri konumlandırmayı öğrendim. Ayrıca menü oluşturmayı ve body 'de arka plan rengi konusunda bazı sıkıntıların nasıl çözüleceğini kavradım. CSS claslarının tek tip yazımı olduğunu düşünürken farklı bir yazımının daha olduğunu bugünki araştırmalarımla edindim.

Şimdi bu öğrendiklerimle beraber yaptığım çalışmalarımı günlüğüme yazacağım.

Bugüne kadar padding ve margin ile hücre içi ve hücre dışı boşluk verme konularıyla divlere konum belirliyordum. Px değerini ayarlamak çok zahmetli bir iştir. Bugün bunun yerine CSS de konumlandırma konusunu öğrendim ve bu komutlarla sayfa içi divlerin konumlarını belirleyeceğim.

Relative değeri divlerin birbirine ve tarayıcıya göre konumlanmaları için kullanılır. Fixed ve absolute ise etiketlerin tarayıcıya göre konumlanmasını sağlar.

Divlerle site yapılacaksa önce en genel container divi ayarlamalıyız. Sayfanın body dışında bütün etiketlerini kaplamalı. Daha sonra header,nav gelmeli ve content olarak bildirilen CSS class’ıyla içerik tanımlaması yapılmalı.Daha sonra bi içerik div'i yazılıp kapatılmalı. En son genel div üzerine footer hücresi yazılmalı ve yan hücre yani aside yazılıp kendi içlerinde kodlanmalı. Bir web sayfası CSS ile beraber genel olarak böyle yapılır bugün bunu öğrendim.


Böylelikle bugün öğrendiklerim beni bir adım dah ileri götürdü. Fakat ben basit bir web sayfası tasarlamak yerine güçlü donanımlı bir web sayfası tasarlamak ve HTML ,CSS dillerine tamamen hakim olmak adına çalışıyorum. Bu yüzden staj süresi dolduğunda proje çalışmama devam edeceğim ve günlük dışında haftalık raporlarımı yine yazacağım.

Daha önce öğrendiğim form oluşturma, tablo yapma gibi konulara bugün web sayfasına menü ekleme ve menülere link verme, oluşturma, header kısmını kodlama logo oluşturmayı da ekleyerek hepsini harmanlayacağım bir alt yapı oluşturdum.

Header kısmında üye girişi, logo, dahili arama motoru olduğunu daha önce öğrenmiştim. Şimdi yine daha önce öğrendiğim basit form sayfalarıyla websayfasının header kısmına bu elementleri eklemeyi amaçlıyorum. Ancak bugün öğrendiğim yeni konu olan konumlandırmaya odaklandım.


Bu gün position özelliğini öğrendim. Position özelliğine

- *Relative*
   - *Float*
   - *Clear*
- *Fixed*
- *Static*
- *Absolute*

Değerleri verip bu özelliğin değerleriyle gerekli konumunu ayarlayabildim. Divler yarattım ve bu divlere bu özellikleri vererek web sayfamda istediğim konumda durmalarını padding ve marginden daha kolay birşekilde yaptım ve sayfa konumunu asıl belirleyen position özelliği olduğunu anladım.

Bu pozisyon özellikleriyle bir anasayfa tasarladım. Bu anasayfamın öncekinden farkı header kısmı kodlanmış, logosu olan, menüsü olan ve position özelliği ile konumlandırılmış olmasıdır. Position özelliğini araştırdığım kadarıyla öğrendiklerim şunlardır:

**Relative:**

Relative divleri birbirine göre konumlandırır.

*FLOAT ve CLEAR:*

Bu iki değer her zamam position: relative ile birlikte kullanılır. Div'lerin yanyana konumlanması için kullanılırlar.

**Fixed:**

Fixed dilimizde sabit anlamına gelir ve sayfanın aşağısına inilse bile kullandığı div aynı konumda kalır.

**Static:**

Static dilimizde durgun demektir. Divleri birbirine göre konumlandırır.

**Absolute:**

Absolute dilimizde mutlak anlamına gelmektedir. Divleri tarayıcıya göre konumlandırır.



Bu gün araştırarak öğrendiğim bu bilgileri harmanlayıp oluşturduğum anasayfa kodlarını aşağıda paylaştım.

**HTML kodları:**


    <html>
        <head><title>Baska Bir CSS</title>
            <link href="bbcss.css" type="text/css" rel="stylesheet"/>
        </head>
        <body>
           <header>
              <fieldset>
                 <a href="http://www.w3schools.com/cssref/logocss.gif"/> <img class="baslik" src="http://www.w3schools.com/cssref/logocss.gif"/</a>
                 <img class="baslik" src="http://www.w3schools.com/cssref/logocss.gif"/>
             </fieldset>
            </header>
            <nav class="ikinci">
                <ul class="liste">
                    <li> <a class="pozisyon" href="#"/> HTML</a></li>
                    <li> <a class="pozisyoniki" href="#"/>CSS </a></li>
                    <li> <a class="pozisyonuc" href="#"/>JavaScript </a></li>
                </ul>
            </nav>
            <div class="calisma">
                  <p class="mavi"><a href="#"/>Bugune padding ve margin ile hucre ici ve hucre disi bosluk verme konulariyla divlere konum belirliyordum. <br/>Px degerini ayarlamak cok zahmetli bir istir. Bugun bunun yerine CSS de konumlandirma konusunu ogrendim ve bu komutlarla sayfa ici divlerin konumlarini belirleyecegim..
       </a></p>
                <p class="yesil">CSS'te konumlandirma belki de CSS'in en onemli konusudur. Eger bu konuyu tam anlamiyla ogrenirseniz CSS'in yuzde ellisini ogrenmis sayilirsiniz. Bu dersimizde static, relative, absolute ve fixed gibi position degerlerini gorecegiz.<br/> Position'a yardimci olan float ve clear ozelliklerini de ogrenecegiz.
           </p>
                  <p class="kirmizi">Bu bir css çalışmasıdır. CSS çalışarak kendimi geliştireceğim ve bu çalışmalarımla web tabanlı programlamaya adım atıyorum.</br> kız arkadaşımla da dertlerim bitmiyo hiçbişeyin normal gittiği yok niye böyle valla bende bilmiyorum.
                  </p>
            </div>
        </body>
    </html>


**CSS kodları:**

    div {
       font-family: Verdana, monospace, sans-serif;
       font-weight: bold;
	   padding:0;
	   margin:0;
       background-repeat:no-repeat;
 	   position:relative;
	   left:170px;
	   }
    .mavi {
       width: 300px;
       background-color: skyblue;
       padding: 20px;
       margin-top: 15px;
	   border-style:solid;
	   font-size:12px;
	   text-align:justify;
	   margin-left:500px;
	   margin-top:-15px;
	   box-shadow: 10px 10px 5px #888888;
	   position:relative;
	   top:50px;
	   text-decoration:none;
       }
    .yesil {
       width: 300px;
       background-color: lightgreen;
       padding: 20px;
       margin-top: 15px;
	   border:solid;
	   border-radius:150px;
	   font-size:12px;
	   text-align:justify;
	   margin-top:-150px;
	   margin-left:20px;
       box-shadow: 10px 10px 5px #888888;
	   position:relative;
	   top:50px;
	   left:50px;
	   }
    .kirmizi {
       width: 300px;
       background-color: lightcoral;
       padding: 20px;
       margin-top: 15px;
	   border:solid 2px;
	   border-radius:200px 150px / 250px 10px;
	   font-size:10px;
	   text-align:justify;
	   padding:40px;
	   margin-top:150px;
	   box-shadow: 10px 10px 5px #888888;
	   position:relative;
	   bottom:50px;
	   left:100px;
	   }
    .liste li {
       display:inline;
       }
    a{
       text-decoration:none;
       text-shadow:1px 2px 5px blue;
      }
    .ikinci{
       text-align:center;
       margin-top:50px;
     }
    .baslik{
       width:150;
	   height:120;
	   background-color:black;
	  }
    .pozisyon{
       position:relative;
       left:-50px;
       font-size:30px;
     }
    .pozisyoniki{
        position:relative;
        left:-5px;
        font-size:30px;
     }
    .pozisyonuc{
       position:relative;
       right:-30px;
       font-size:30px;
     }

Bu gün CSS'de konumlandırmayı öğrenerek ilerleme kaydettim. Daha sonraki çalışmalarımda geçmiş bilgilerimi ve öğrendiğim yeni bilgileri harmanlayarak devam edip kendimi geliştireceğim.
