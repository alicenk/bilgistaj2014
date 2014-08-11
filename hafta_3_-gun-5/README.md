# Üçüncü hafta
##5.gün
**08/08/2014**

Bu gün CSS komutlarından bazılarını inceledim. Ne işe yaradıklarını araştırdım. Syntax'ı iyice kavramak için öğrendiklerimi kendim yazıp notepad++ editöründe çalıştırıp denedim. Bu günki çalışmalarımdan sonra CSS stillerini farklı tekniklerle çağıracağım. Web sitemin ana sayfasını tasarlamaya başlayacağım.

Öncelikle CSS'in ortaya çıkışını araştırdım ve W3C oluşumunu öğrendim. Tarihçe bakımından CSS de yine bir ihtiyaç dahilinde ortaya çıkmış oluşturulmuş bir yaklaşımdır. HTML'de kargaşayı azaltmak, kod kalabalığına son vermek adına CSS stilleri oluşturmak için, still dosyalarının dışarıdan çağırılmasını sağlamak adına oluşturulmuştur.

World Wide Web Consortium (dünya çapında ağ konsortiyum),  Tim Bernes Lee tarafından kurulan web’in gelişmesinde katkıda bulunan bir oluşumdur. WC3’de birçok yazılımcının etkisi vardır ve standart amacı farklı va sabit amaçlar belirlemiş tarayıcıların aynı stiller için aynı sonuçlar üretmesini, benzer görünümler içermesini sağlamaktır.Bu oluşum HTML çıktılarının belirli bir standartta olmasını sağlamaya çalışır.


CSS'in syntax'ını bir önceki gün incelemiştim. Hatta daha önce HTML çalışırken de CSS dosyasının nasıl çağırıldığını, kod içine nasıl yazıldığını, kendi tag'ıyla HTML içine nasıl yazıldığını irdelemiş ve bu yöntemlerden en kullanışlısının link tag'ıyla CSS dosyası çağırmak olduğunu öğrenmiştim. Şimdi bunların üstüne CSS komutları nasıl yazılır ve çıktıları nelerdir bunları icraate dökerek çalışacağım ve daha iyi kavrayacağım.

***CSS'de class kullanımı:***

HTML tagları için stil belirleyebildiğimiz gibi kendimize özel stiller belirleyip elementlerin id ve class özelliklerinde bu stili belirterek de kullanabiliriz.

     <div class=”stil”> Hoş geldiniz</div>


Yukarıdaki div elementi içinde yer alan class=”stil” o div elementi için css özelliklerini belirmememizi sağlayan bir yoldur.


Bu elementin çağırıldığı class şudur


    .stil{
       Font:10pt;Thoma, Veranda;
       Color:blue;
     }


. ile başlayan bir stil oluşturduk. Bu class=”stil” ise belirttiğimiz tüm elementler bu özellikde olacaktır. Eğer bu özelliklerin tek element için geçerli olmasını istiyorsak .stil başına istediğimiz elementin adını yazmamız yeterlidir.

Class özelliğini kullanmanın bize sağlayacağı faydalar şunlardır:

- Kendi adlandırdığımız özel stiller yaratabilir ve bunları kullanabiliriz.
- Bir stili birden fazla elementte kullanabiliriz.(Öteki türlü her element için farklı stiller yazmak gerekiyordu.)
- Stilleri CSS'de yazarak HTML kodlarımızda sürekli tekrarlardan ve kod kalabalığından kurtarabiliriz.

***CSS'de ID kullanımı:***

ID özelliği ile de stiller yaratabiliriz. Classtan farkları şunlardır:

- Sadece tek bir elemette kullanabiliriz. Birden fazla elementte kullanılmaz.

   - Bunun sebebi ID'nin identity kelimesinden gelmesidir.Identity kelime anlamı olarak adres demektir ve sadece gitmesi gerektiği elementi belirtir.

- Stil dosyamızda CLASS'da . (nokta) kullanırdık, ancak id özelliğine göre stilleme yapacaksak # (diyez) kullanırız.


Bu özellikleri örnek üzerinde görücek olursak:

    <div id=”stil”> hoşgeldiniz</div>

CSS dosyamızda bu elemente göre özel stil tasarlarken aşağıdaki kod yapısını oluşturmalıyız:

    #stil {
      Font:10pt; Thoma, Veranda; color:blue;
     }

ID, HTML dosyasında o elementi bulmamızı sağlar, bu nedenle aynı ismi veremeyiz. Aynı ismi vermemizin diğer yaratacağı sorun Java Script'te bu elementi id özelliğine göre kullanamamak olacaktır. Son olarak bazı tarayıcılar birden fazla aynı id kullanılan HTML dosyalarında stilleri görmezden gelebilir.

CSS dosyasının HTML kodlarında en çok kullanım şekilleri:
- link yöntemiyle (< link href=”cssdosyasi.css” type=”text/css” rel=”stylesheet”/ > )
- HTML sayfasına CSS yazmak dışında bir de html elementinin içerisinde stil belirterek kullanılması.

         <html>
            <head>
               <title> Sayfa Başlığı </title>
               <style type="text/css">
                 body{
                      background-color:black
                      }
                  p {
                      font-family:Tahoma,Verdana;font-size:12px;
                      }
                </style>
            </head>
            <body>
                <p>Bu 12 pixel tahoma yazı tipiyle yazıldı</p>
            </body>
         </html>

Bu yöntem ile HTML kodlarının içine CSS kodu yazıldı. Bunun için HTML'nin 'style' tag'ından yararlanıldı.

HTML taglarının içeririsine style belirtmenin yöntemi ise şudur:

         <p style="font-family:tahoma;font-size:12px;">
         Bu 12 pixel tahoma yazı tipiyle yazıldı.
         </p>

Bu yöntem sadece hızlı çözüm gerektiği zamanlarda kısa bir çözüm olmasından dolayı kullanılabilir.

***CSS ile arka plan:***

Background özelliği elemanın arka planıyla ilgili değişiklik yapılmasını sağlar.
Background-color özelliği elemanın arka plan rengini belirtir.
Background-image özelliği bir elemanın arka plan olarak kullanmak üzere bir görüntüyü belirtir.

Resim için

Body{
Background-image: url(“resim.jpg”);
}

Syntax budur.


Repeat tekrar demektir.Bir arkaplan yatay tekrarlanmak istenirse arka plan özelliği background-repeat: repeat-x; olmalıdır. Düşey olması için repeat-y olmalıdır.Eğer arka plan tekrarı istemiyorsak background özelliğini no-repeat olarak değiştiririz.
Arka plan olarak background özelliklerini tek tek girmek yerine background: dan sonra özellikleri tek tek girebiliriz.


Arka plan olarak background özelliklerini tek tek girmek yerine background: dan sonra özellikleri tek tek girebiliriz.Buna 'steno' özelliği denir.

Belirlediğimiz elemanın konumu için kullanılan özellik background-position’dır.

Text-decoration özelliği ayarlamak veya metinden süslemeleri kaldırmak için kullanılır.
Text-decoration özelliği çoğunlukla tasarım amaçlı linklerden altçizgilerini kaldırmak için kullanılır.

     <!DOCTYPE html>
    <html>
      <head>
        <style>
          a {
            text-decoration: none;
            }
       </style>
     </head>
     <body>
       <p>Link to: <a href="http://www.w3schools.com">W3Schools.com</a></p>
      </body>
    </html>

Bu kod ile < head > tag'inde yazılan a tag'ı için kullanılması komut verilen CSS kodu sayesinde verilen linkte normalde alt çizgi olması beklenirken alt çizgi görünmicektir.

Bknz:

<!DOCTYPE html>
<html>
<head>
<style>
a {
    text-decoration: none;
}
</style>
</head>
<body>

<p>Link to: <a href="http://www.w3schools.com">W3Schools.com</a></p>

</body>
</html>


Bu görevi gördüğü gibi tam tersi metinleri dekore etmek amaçlı çizgilerin yerini de belirtebilir.

Text-indent özelliği, bir metnin ilk satırının girinti belirtmek için kullanılır.

      p {
         text-indent: 50px;
        }

Metinin konumunu belirlemek için kullanmamız gereken özellik text-aling özelliğidir. HTML’de incelediğim < center > etiketi burada özelliğin değeri olarak işlev görür.

Bu gün CSS kodlarına genel giriş yaptım. 4.haftada farklı bir kaynaktan çektiğim buton kodunu notepad++'da derlediğimde butonlarım düz çıkmıştı.Sebebini ilerki haftalarda irdeleyeceğimi söylemiştim. Şimdi orada görüntünün istediğim gibi olmamasının sebebinin CSS kodları olduğunu anladım. Her bir buton için farklı büyüklük ve mavi renk almak için CSS kodları gerekliydi.

Bu gün üçüncü haftamın son günü. Stajımın bitmesine kalan 8 iş günümde taslak anasayfamı oluşturmaya çalışacağım ve bunun için CSS kodlarını daha çok irdeleyeceğim.
