#Birinci hafta
## 4. Gün
**24/07/2014**

Bugün css ile html bağlantısına biraz giriş yaptım. Bazı websitelerde açıklamaları okudum bootstrap framework'ün ne işe yaradığını araştırdım. Github sayfasından bootstrap'ı indirdim. Css'e biraz daha hakim olabilmek için bazı hazır kodları inceledim ve burada yapılan işlemlerden projeme katkıda bulunacağım. Hazır kodları ve çıktılarını inceledim. Html kodlarına css kodlarının nasıl çekilebileceğine dair birkaç yöntem inceledim. İncelediğim yöntemler başlık halinde şunlar:

- Kod içinde (İn-line)
- Style elementi kullanarak
- Harici style şablonu kullanımı
- @import ile eklemek


***Kod İçinde:***

Direk olarak HTML elementinin içine style özelliği kullanılarak uygulanır.


    <div style="color:red">Deneme yazımız</div>
Bu kod css'in style yöntemiyle yazılmış ve notepad++ da yazıp farklı kaydettikten sonra .html uzantısıyla herhangi bir tarayıcıda çalıştırırsak ekranda kırmızı renkte "deneme yazımız" yazısını göreceğiz.

***Style elementi kullanarak:***

< head > kısmına < style > elementi kullanarak CSS kodu yazarak uygulamak.

    <html xmlns="http://www.w3.org/1999/xhtml">`
       <head>
       <meta http-equiv="Content-Type" content="text/html; charset=iso-8859-9" />
        <title>CSS'i Uygulamak </title>
        <style type="text/css">
        div{
           color:red;
        }
        </style>
      </head>
    </html>

< head > </ head> kısmına bu kodları yazdığımızda, css komutlarını yerleştirdiğimizde çalıştırdıktan sonra ekranda kırmızı olarak "CSS'i uygulamak" yazmaktadır. CSS komutlarının çoğunluğu html kodlarının < head > kısmında bulunmaktadır.




***Harici style şablonu kullanımı:***

Bu metodla CSS komutlarımızı herhangi bir editörde yazdıktan sonra .css uzantılı olarak kaydederiz. HTML kodlarımızı yazarken gereken yerde çağırırz.

Yani CSS ile özellikler bir dosyada kaydedilir. Bu özellikler kodlamada HTML kodlarıyla çağırılarak kullanılır. En büyük avantajı bir kere yazılan kod lazım olan tüm sayfalara eklenebilmesidir. Bu sayede harici eklenen css kodu bir kere yüklendikten sonra diğer kullandığımız sayfalarda tekrar yüklenemeyerek bize hız kazandıracaktır.

    p {
    color: red;
    }
    a {
    color: blue;
    }

Örnek bir css kodunu HTML satırında uygun herhangi bir yöntemle çağırabiliriz.

    <html xmlns="http://www.w3.org/1999/xhtml">
         <head>
            <meta http-equiv="Content-Type" content="text/html; charset=iso-8859-9" />
            <title>CSS'i Uygulamak</title>
            <link rel="stylesheet" type="text/css" href="ornek.css" />
         </head>
     </html>

Link elementiyle HTML kodlarına CSS komutları eklenmiş,çağırılmıştır. Bir kere yazılan CSS kodu bu çağırma yöntemiyle lazım olan bütün sayfalara çağırılabilir.

***@import ile eklemek:***

    <html xmlns="http://www.w3.org/1999/xhtml">
         <head>
         <meta http-equiv="Content-Type" content="text/html; charset=iso-8859-9" />
            <title>CSS'i Uygulamak</title>
            <style type="text/css">
            @import "ornek.css";
            </style>
          </head>
     </html>

Örnek bir html kodudur ve @import yöntemi ile ornek.css dosyasında css komutları çağırılır. 3.yöntem ile benzerliği vardır ancak @import ile eklenen kod link ile eklenen koddan daha çabuk yorumlanır. Bu yüzden eski web tarayıcıları tarafından görülmeyebilir.

Bu gün bootstrap ile CSS komutlarını araştırdım. HTML kodlarına CSS komutlarının nasıl dahil edileceğini öğrendim ve bununla alakalı yöntemleri araştırdım. Elde ettiğim 4 yöntem sayesinde projemde css komutlarını çalıştırabileceğim.

