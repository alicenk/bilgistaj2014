#Beşinci hafta
##Üçüncü gün
**20/08/2015**


Bugün stajın son günü. Staj boyunca bir web sayfasının genel yapısını, web tasarımın temellerini, sürüm kontrol sistemini ve temel olarak HTML,CSS dillerini öğrendim. JavaScript hakkında bilgi sahibi olabilecek kadar birikim sağladım.Şöyle ki yaptığım çıkarımlar doğrultusunda HTML bir vücudun iskeletiyse CSS vücudun dış görünüşünde karar kılan HTML'i şekillendiren bir web teknolojisidir.JavaScript ise vücudun fonksiyonlarını belirleyen, davranışlarını kontrol eden yazılım dilidir.

Bu gün son günüm olması dolayısıyla çalışan arkadaşlarımla vedalaştım. Günlüklerimi kontrol ettim ve anasayfamı inceleyip kodlarımı düzenledim. Geliştirdiğim oldukça basit anasayfa projeme bilgilerim dahilinde kendimi gelitirmek adına stajımdan sonra da devam edeceğim.

HTML ve CSS öğrenerek web tasarım konusunda temel oluşturdum. Artık kolaylıkla yarı profesyonel bir web sayfası oluşturabilirim.

Stajımda son olarak kısaca sözde eleman ve özellik seçici konularında çalışmalarıma devam ettim.

Sözde eleman syntax'ı şudur:

    eleman tanımlayıcı(HTML etiketi)::sözde eleman {
        özellik:değer;
    }

CSS class'ları da sözde elemanlarla birlikte kullanılır.Yani HTML elemanını class'ıyla tanımlarsak o class'a bağlanır.Bunu daha iyi anlayabilmek için notepad++'dan boş bir sayfa açıp şu kodları yazıp çalıştırdım.

     <html>
        <head>
           <title>Yine bir deneme</title>
           <style>
             p.article::first-letter {color:#ff0000;}
           </style>
        </head>
        <body>
           <p class="article">Makalede bir paragraf</p>
        </body>
     </html>

Bu kodları çalıştırdığımda < p > etiketinin içine yazdığım cümlenin ilk harfini çok büyük olarak gösterdi.

Bu çalışmayla ::first-letter sözde elemanının textlerin ilk harflerinde değişiklik yaptığını öğrendim.

::first-letter yerine ::first-line kullandığımda ise bütün satırda değişiklik oluyordu. Bu şekilde ::first-line sözde elemanının sadece satırda değişiklik yapmaya yaradığını öğrendim.

Daha sonra sözde elemanlardan ::before elemanının daha olduğunu öğrendim. Bu eleman web sayfasına dahil olduğu textlerden önce bir ifade koyuyordu.

Daha iyi anlamak için aşağıdaki kodları yazdım ve çalıştrdım.

    <html>
      <head>
        <style>
           h1::before {
           content: url(smiley.gif);
               }
        </style>
      </head>
      <body>
         <h1>Bu bir başlık</h1>
         <p>::before sözde elemanı öğeden önce içeriği ekler </p>
         <h1>Bu bir başlık</h1>
      </body>
    </html>

Kodlarını çalıştırdığımda head taglarına yazılan textlerden önce gülümseyen ifade görünüyordu.

Before yerine ::after sözde elemanını kullandığımda ise textten sonra ifadenin oluştuğunu gördüm.

Daha sonra CSS'de özellik seçici konusunu biraz inceledim. Kodlarına baktığımda kendi irademizle class oluşumu gibi geldi.

    [özellik] {
       font-weight: bold;
       text-decoration: underline;
     }
Bu örnek syntax'a benzer bir syntax'ı olduğunu gördüm. Class çağırımından farklı bir çağırımı vardır. Şöyle ki:

     <div özellik>
        <p>Bu bir denemedir.</p>
     </div>
Kodlarını yazdığımda özellik adlı seçicide tanımlanan CSS komutlarını websayfamda görebildim.

Aynı özellik seçici ismiyle farklı özellik seçicileri class çağırımına bire bir aynı yöntemle çağırılabildiğini gördüm. Şöyle ki:

     [özellik="a"] {
           color: green;
          }
     [özellik="b"] {
           color: maroon;
          }

Bu CSS kodlarının HTML kodlarında kullanımı şu şekildedir:

    <div özellik="a">
        <p>Bu bir denemedir.</p>
    </div>
    <div özellik="b">
        <p>Bu bir denemedir.</p>
    </div>

Özellik seçicileri kullanarak classlara benzer yöntemlerle CSS kodlarını çağırabildim.

Son günde çalıştığım bu uç bilgilere bundan sonraki dönemlerde de eklemeler yapacağım. Burada oluşturduğum HTML ve CSS temeline yeni bilgiler ekleyip web programlama konusunda kendimi geliştireceğim. Stajın son gününde 20 günlük iş deneyimimle kendime web programlama adına sağlam bir temel oluşturdum.
