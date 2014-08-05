# 4. Gün

**24/07/2014**


Bugün css ile html bağlantısına biraz giriş yaptım.Birkaç websiteden araştırma yapıp bootstrao framework'un ne işe yaradığını araştırdım.GitHub sayfasından bootstrap'ı indirdim.Css'e biraz daha hakim olabilmek için bazı hazır kodları inceledim ve burada yapılan işlemlerden projeme katkıda bulunacağım. Hazır kodları ve çıktılarını inceledim. Html kodlarına css kodlarının nasıl çekilebileceğine dair birkaç yöntem inceledim. İncelediğim yöntemler başlık halinde şunlar:

* Kod içinde(İn-line)
* Style elementi kullanarak
* Harici style şablonu kullanımı
* @import ile eklemek

***Kod İçinde:***

Direk olarak HTML elementinin içine style özelliği kullanılarak uygulanır.

< div style ="color:red">Deneme yazımız < /div >

Bu kod css'in style yöntemiyle yazılmış ve notepad++'da yazıp farklı kaydettikten sonra .html uzantısıyla herhangi bir tarayıcıda çalıştırırsak ekranda kırmızı renkte "deneme yazımız" yazısını göreceğiz.

***Style elementi kullanarak:***

< head > kısmına < style > elementi kullanarak CSS kodu uygulamak.

       < html>
         < head >
           < meta     http-equiv="content-type"content="text/htmk;charser=iso-8859-9 " />
         < title > CSS'i uygulamak < / title
         < style type = "text/css" >
         div {
         color:red;
        < /style >
        < /head >
       < /html >

Bu örnek kodları notepad++'da .html uzantısıyla kaydedip herhangi bir tarayıcıda çalıştırdığımızda websayfasında yine kırmızı renkte "CSS'i uygulamak" yazıcaktır. Ancak 'title' etiketine yazdığımız için websayfasının başlığı olarak görünücektir.

***Harici style şablonu kullanarak:***

Bu metodla CSS komutlarımızı herhangi bir editörde yazdıktan sonra .css uzantılı olarak kaydederiz. HTML kodlarımızı yazarken gereken yerde çağırırz.

Yeni CSS ile özellikler bir dosyada kaydedilir. Bu özellikler kodlamada HTML kodlarıyla çağırılarak kullanılır. En büyük avantajı bi kere yazılan kod'un lazım olan tüm sayfalara eklenebilmesidir. Bu sayede harici eklenen css kodu bir kere yüklendikten sonra diğer kullandığımız sayfalarda tekrar yüklemeyerek bize hız kazandıracaktır.

         p{
        color:red;
         }
        a{
        color:blue;
         }

Örnek bir css kodunu HTML satırında uygun herhangi bir yöntemle çağırabiliriz.Yukarıdaki örnek css kodunu .css uzantısıyla ornek.css adıyla kaydedersek aşağıdaki şekilde çağırabiliyoruz.

         <hml>
           <head>
           <title> CSS'i uygulamak </title>
           <link rel="stylesheet" type="text/css"             href="ornek.css" />
           </head>
          </html>



Link elementiyle HTML kodlarına CSS komutları eklenmiş,çağırılmıştır. Bir kere yazılan CSS kodu bu çağırma yöntemiyle lazım olan sayfalara çağırılabilir.

***@import ile eklemek:***

     < html >
       < head >
       < title > CSS'i uygulamak < /title >
       < style type = "text/css" >
        @import "ornek.css";
        < /style >
        < /head >
    < /html >


Örnek bir html kodudur ve @import yöntemiyle css komutlarının nasıl çekilebildiğini gösterir. 3.yöntem ile benzerliği vardır ancak @import ile eklenen kod link ile eklenen koddan daha çabuk yorumlanır.Bu yüzden eski web tarayıcıları tarafından görülmeyebilir.
