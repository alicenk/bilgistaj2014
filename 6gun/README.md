#İkinci hafta
##1.gün
**31/07/2014**

Bugün HTML kodlarını iyice kavramak adına temel HTML kodlarını inceleyip basit taslak bir website tasarladım. HTML'ye iyice hakim olmak adına notasyonu kavrayabilmek için böyle çerez siteler programlar yapıp derleyeceğim. Daha sonra CSS dosyasını çekip,kodları karıştırıp nasıl olduğunu öğreneceğim. HTML ile sade bir web site tasarlamak isterken ve elementlerinin,komutlarının ne işe yaradığını araştırırken HTML ile ilgili bazı bilgiler edindim.

HTML , Hyper Text Markup Language kelimelerinin baş harflerinin kısaltması olan, türkçe ifade ile "zengin metin işaretleme dili"dir. HTML CERN'de müteahhit olarak çalışan Tim Berners-Lee tarafından 80'li yıllarda geliştirilen, 90'lı yıllarda ise adının konduğu bir web standartıdır.

HTML'de bağlantılar (link'ler) < a > etiketi içine yazılır. a harfi İngilizce'deki attribute kelimesinin kısaltmasıdır. Dilimizde "atıf" gibi bir anlama gelmektedir.

   < a href="http://www.google.com.tr/">Bu bir link'tir.< a >

Bu kod satırı web sayfamızda link vermeye yarar ve href'den sonra = yazdığımızda tırnak içine yönlenmek istediğimiz sitenin adını yazarız.
 `<img src="http://görseliçerik.com"/>`

Bu örnek kod satırıyla tırnak içine görsel birşey içeren link yazdığımızda çalıştırdığımız zaman web sayfamızda linkteki görsel içerik görünür.

Bu bilgiler yardımıyla aşağıdaki kodlarla birlikte örnek taslak bir websitesi elde ettim.

            <html>
            <head>
            <title> çiçekler</title>
            </head>
            <body>
            <h1>Çiçekler türleri</h1>
            <Phasellus feugiat ligula vitae purus pretium nec commodo lorem convallis.</p>
      <h2>Kırmızı Çiçekler</h2>
      <img src="http://www.zinzinzibidi.com/Areas/web_tasarim/Content/img/cicek.png" alt="kırmızı bir çiçek" />
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis quam mi,.</p>
      <p>Curabitur sit amet arcu ac lectus aliquet placerat. Duis sit amet.</p>
      <h2>Mavi Çiçekler</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla leo.</p>
      <a href="http://www.zinzinzibidi.com/Areas/web_tasarim/Content/img/mavi_cicek.jpg">Mavi bir çicek örneği</a>
      </body>
      </html>













Bu kodlar notepad++'da .html uzantısıyla kaydedilip bir web tarayıcıda çalıştırıldığında oluşan web sayfasında kırmızı çiçek başlığının altında verdiğim linkten kırmızı çiçek resmi oluştu. Mavi çiçek içinse direk link'i web sayfasında oluşturduğumuz için linke tıklayarak ulaşılacak.

<html>
    <head>
    <title>Çiçekler</title>
    </head>
    <body>
    <h1>Çiçekler Türleri</h1>
    <p>Phasellus feugiat ligula vitae purus pretium nec commodo lorem convallis.</p>
    <h2>Kırmızı Çiçekler</h2>
    <img src="http://www.zinzinzibidi.com/Areas/web_tasarim/Content/img/cicek.png" alt="kırmızı bir çiçek" />
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis quam mi,.</p>
    <p>Curabitur sit amet arcu ac lectus aliquet placerat. Duis sit amet.</p>
    <h2>Mavi Çiçekler</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla leo.</p>
    <a href="http://www.zinzinzibidi.com/Areas/web_tasarim/Content/img/mavi_cicek.jpg">Mavi bir çicek örneği</a>
    </body>
    </html>

