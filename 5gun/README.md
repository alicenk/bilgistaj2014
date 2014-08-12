#Birinci hafta
##5.gün

**25/07/2014**

Stajımın ilk haftasının son gününde genel hafta tekrar ve bazı CSS frameworklerini araştıracağım. Haftann sonunda edindiğim bilgilerle HTML kodlarıyla basit bir web sitesi tasarlayarak projeme başlayacağım. Daha sonra edindiğim bilgileri kafamda tasarladığım twitter clonu bir websitenin tasarım aşamasına başlayacağım.


Bu gün CSS komutlarıyla tasarlanmış basit web site örneklerini inceledim. CSS ile web sayfasına form, buton yerşleştirmeyi vurgulu yazıları sayfada görüntülemeyi öğrendim.


İncelediğim html kodlarında html çalışırken projemde işime yarayacak bazı kodları çekmeyi düşünüyorum. İncelediğim kodlardan bazıları ve sayfa görüntülerini aşağıda sıraladım.

         <html>
           <head>
              <link rel="stylesheet"href="docs/assets/css/bootstrap.css">
              <link rel="stylesheet/less" href="less/bootstrap.less">
            </head>
            <body>
              <div class="container">
               <div class="span9">
             <div class="hero-unit"
                <p> MERHABA DÜNYA</p>
            </div>
           </div>
          </body>
         </html>


Link yöntemiyle bootstrap'tan css dosyası çekilmiştir. İlgili kod ise şudur.

            <link rel="stylesheet"href="d0s/assets/css/bootstrap.css">
            <link rel="stylesheet/less" href="less/bootstrap.less">

 Bu kodlara ait ekran çıktısı arka planı gri olan websayfasında yazan MERHABA DÜNYA olacaktır.


 Web sayfasında uyarı,hata,sessiz,başarı gibi vurgu yazılarını ekranda gösteren kodlar şunlardır:

         <p class="muted"> sessiz.</p>
         <p class="text-warning">uyarı.</p>
         <p class="text-error">hata.</p>
         <p class="text-info" >haber.</p>
         <p class="text-success">başarı.</p>

Bu kodları notepad++ da .html uzantısıyla kaydettiğimizde  websayfasında


<p class="muted"> sessiz.</p>
<p class="text-warning">uyarı.</p>
<p class="text-error">hata.</p>
<p class="text-info" >haber.</p>
<p class="text-success">başarı.</p>

Çıktısını alırız.


Kullanıcı adı, şifre, e-posta isteyen bir web arayüzü için gerekli kodlar:


         <form class="form-horizontal">
            <div class="control-group">
              <label class ="control-label" for="inputEmail">Email</label>
               <div class="controls">
                <input type=text id="nputEmail" placeholder="Email">
               </div>
               </div>
             <div class="control-group">
              <label class="control-label"
             for="inputPassword">Password</label>
               <div class="controls">
                <input type="Pasword" id="inputPasword"
                 placeholder="Pasword
                </div>
               </div>
             <div class="control-group">
               <div vlass="controls">
                 <label class="checkbox">
              <input type="checkbox"> remember me
             </label>
             <button type="submit" class="btn">Sing in </button>
             </div>
             </div>
         </form>



 Bu kodlar notepad++'da .html uzantısıyla çalıştırıldığında web sayfamızda bir form sayfası ve kullanıcıdan e-posta ve şifre isteyecek metin kutuları görünecektir. Bir de chechbox olacaktır orda da 'remember me' ifadesi bulunacaktır.


 Ben bu kodlarla genel bir form yapısını, websayfamda olucak olan uyarı ibarelerini  bunların nasıl koda döküleceğini bu kodlarla inceledim fikir sahibi olmaya çalıştım. Şimdi de sade bir html çalışmasıyla kendim websayfasına buton ekledim. Benim kodlarım da şunlar:

         <html>
         <head>
         <title>Sayfaya buton ekleme</title>
         </head>
         <body>
         <p>Submit gönderme, reset sıfırlama butonudur.</p>
         <input type="Submit"/p>
         </body>
         </html>

Bu kısa kod çalışmamın ilerki çalışmalarıma öncü olacağını ümit ediyorum.Title elementi ile websayfamın başlığını "Sayfaya buton ekleme" olarak belirledim.Paragraf olarak açıklama anlamında Submit kısmının gönderme, reset'in ise sıfırlama butonu görevini gördüğünü söyledim.Butonu oluşturacak kodu ise yazdığımda "Submit" yazdığım için gönderme butonu oluşucaktır.





 Bugün bağımsız olarak öğrendiğim diğer bir program da websayfasında tablo oluşturma programı oldu. Oluşturduğum tablonun kodları şunlar:

         <html>
          <head>
            <title>tablo</title>
          </head>
          <body>
            <table border=10>
             <tr>
              <th>Sıra no</th>
              <th>isim</th>
              <th>soyisim</th>
              <th>yaş</th>
             </tr>
             <tr>
              <td align="center">1</td>
              <td>ahmet</td>
              <td>doğru>/td>
              <td>21>/td>
             </tr>
             <tr>
              <td align="center">2</td>
              <td>can</td>
              <td>tezcan</td>
              <td>23</td>
             </tr>
             <tr>
              <td aling="center">3</td>
              <td>gökalp</td>
              <td>turgut</td>
              <td> 24</td>
             </tr>
           </body>
         </html>

Bu kodlamada tablo yaparken gerekli elementlerin neler olduğunu öğrendim. Tablonun kalınlığını body kısmında  table etiketinin border özelliğinin belirlediğini öğrendim. Tablodaki nesneleri ortalamak için de "align center" komutunu kullanmamız gerektiğini öğrendim. Eğer nesnelerin sağda olmasını istersek "align center" yerine "align right" yapmamız gerektiğini öğrendim. Başlıklar için diğerlerinden ayrı olarak < th > elementini kullandık. Ancak yine < td > kullanarak bunun içerisinde başlık elementi olan < h > kullanabilirdik. Sayfanın görüntüsü aynı olurdu.



Tablo yapmak için < table > < /table > komutunun içine < tr > < /tr > komutunun gerekliliğini öğrendim.

Bir önceki kendi sade çalışmamda tek buton yapmıştım. Şimdi ise araştırıp CSS komutlarıyla farklı büyüklüklerde butonların nasıl yapıldığını, kodlandığını öğrendim. Bu gün incelediğim kodlardan sonuncusunu söylemeden önce kaynak olarak aldığım site şudur: http://tugdev.github.io/



    <button type="button" class="btn btn-large">Large button</button>

    <button type="button" class="btn btn-primary">Default button</button>
    <button type="button" class="btn">Default button</button>

    <button type="button" class="btn btn-small btn-primary">Small button</button>
    <button type="button" class="btn btn-small">Small button</button>

    <button type="button" class="btn btn-mini btn-primary">Mini button</button>
    <button type="button" class="btn btn-mini">Mini button</button>

 Bu kodları notepad++'da çalıştırdığımda görmek istediğim sayfa görüntüsü solda large button isimli mavi renk buton, sağda gri renkli large buton isimli buton olmasıydı. Aşağı doğru küçülmesini bekliyordum ancak tarayıcıda karşılaştığım görüntü düz butonların sıralaması oldu. Bu sorunu css'e daha derinlemesine girdiğimde araştıracağım.


