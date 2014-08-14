#Dördüncü hafta
##3.gün
**13/08/2014**

Bu gün hücrelerin sınırlarına, farklı CSS çekme yöntemlerine, önceki CSS bilgilerimi pekiştirmek amaçlı text özelliklerine yönelik çalıştım.

Hücre içi ve dışı boşluklar yani marjlar hakkında derin araştırma ve deneme yanılma yöntemiyle kesin, önemli ve net bilgilere ulaşarak kafamdaki soru işaretlerini tek tek sildim.

Öncelikle bir tablo oluşturarak o tabloda padding ve margi değerlerini CSS kodlarından çekmeyi denedim. Ancak tablonun bir bölümünün etiketine uyguladığım da verdiğim özelliklerden padding'in diğer etiketleri de etkilediğini, margin'inse hiçbirini etkilemediğini gördüm.

Bunun sebebi örneğin div etiketinde padding değerler girdiğimizde içerideki text'in konumu değişiyor ancak div hücresinin içinde değişime uğruyor. Div bir web sayfasının tag'ı olduğu kadar bölümü ve hücresidir. Ancak tablo içerisinde bir etikete padding değerler verdiğimde div nasıl değişiyor, genişliyor ya da daralıyorsa tablo etiketi olan td de o şekilde daraldı ve genişledi. Ancak padding-top ya da padding-bottom yaptığım zaman tablonun konumu da değişiyordu. Bunun sebebi td etiketinin ait olduğu hücre table yani tablodur. Tablo içerisinde kendisine bağlı etiketleri de kendi konumuyla değiştirebilir.Bunun ayrıntılı açıklamasını günlüğüme yazacağım.

Daha sonra menü oluşturmak için satır içi listeleme kodlarını araştırdım. Bunu araştırırken kaynak olarak kullandığım editördeki kodlarla kendim oynayarak eski bilgilerimi pekiştirdim. Daha sonra nav tag'ıyla web sayfasındaki menü görünümünü oluşturmaya çalışacağım. Şimdi edindiğim bilgileri günlüğüme yazacağım.


Her hücre kendi sınırlarını oluşturur. Yani bir hücre içerisinde padding oluşturursak eğer bu padding’e özellikler veririz ve sayfadaki konumunu oluştururz. Fakat etiket içindeki etikete sınır verdiğimizde yani tablo gibi bir etiketin td etiketine bir CSS dosyası yüklediğimizde onun hücresi yani div’i tablo olduğu için div içerisinde tablo tanıtıldığı için padding özellikleri yani div içerisinde verilen padding özellikleri içerideki özeliği verilen tag’ı div içerisinde oynatır. Yani demek istediğim padding ve margin hücre içi veya dışı boşluktur. Etiketlerde kullanırsak o etiketin dahil olduğu hücre içindeki yerini belirlemiş oluruz.

Örnek vericek olursak şu kodlara bir bakalım:

    <html>
        <head>
            <style>
                p {
                  background-color: yellow;
                  }
                p.ex {
                  margin-top: 150px;
                  margin-bottom: 100px
                  margin-right: 150px;
                  margin-left: 50px;
                    }
            </style>
        </head>
        <body>
            <table>
                <tr>
                <td>
                   <p>This is a paragraph with no specified margins.</p></td>
                <td><p class="ex">This is a paragraph with specified margins.</p></td>
                </tr>
            </table>
        </body>
    </html>

Bu kodlarda tablo değerinde < td > tagında hangisinde class çağırıldıysa onun için css kodları geçrlidir. Ancak tablo elementi bu iki elementi de sınırladığından dolayı bir elementin yeri değişince diğeri de değişir. Tablo olmadığını varsayarsak:

    <html>
        <head>
            <style>
                p {
                   background-color: yellow;
                   }
                p.ex {
                  margin-top: 100px;
                  margin-bottom: 100px;
                  margin-right: 150px;
                  margin-left: 50px;
                  }
            </style>
        </head>
        <body>
            <p>This is a paragraph with no specified margins.</p>
            <p class="ex">This is a paragraph with specified margins.</p>
        </body>
    </html>

Bu durumda sadece çağırılan element için CSS komutları yerini değiştirir. Yani bir element diğer elementleri etkileyecekse tablo gibi birbirine bağlı elementleri etkileyecekse CSS sadece onun için çağırılmış olsa bile diğerlerinin yeri değişecektir.

Bu yüzden div’ler yani hücreler tanımlamalıyız ve web sayfasındaki konumu bu birbirine bağımsız hücrelerle belirlemeliyiz. Bu şekilde birbirlerini etkilemeyeceklerdir.

Margin özelliği bir ila dört değere sahip olabilir.

-  **margin 25px 50px 75px;**
    - Üst kenar boşluğu 25px olduğunu
    - Sağ kenar boşluğu 50px olduğunu
	- Alt kenar boşluğu 75px olduğunu
	- Sol kenar 100px olduğunu

- **margin: 25px 50px 75px;**
    - Üst kenar boşluğu 25px olduğunu
	- Sağ ve sol kenar boşlukları 50px vardır
	- Alt kenar boşluğu 75px olduğunu
- **margin: 25px 50px;**
    - Üst ve alt kenar boşlukları 25px vardır
	- Sağ ve sol kenar boşlukları 50px vardır
- **margin: 25px;**
    - dört kenar vardır 25px

Paragraflar arasında boşluk bırakmak istiyorsak da marj kullanabiliriz. Yani margin belirtebiliriz ve margin’e sadece pixel değeri vermek zorunda değiliz. Margin bulunduğu etiketin ya da hücrenin sınır değerlerini değiştirir ancak o etiket başka bir etikete bağlıysa bağlı olduğu etiketin sınır değerlerini etkilediğinde bağlı olduğu etiketin yeri de değişir. Bu yüzden bağımsız taglarda kullanılması en mantıklısıdır.Aşağıdaki kod satırlarında olduğu gibi margine bir cm değeri verebiliriz.

    <html>
        <head>
            <style>
               p.ex1 {
                  margin-top: 2cm;
                     }
            </style>
        </head>
        <body>
              <p>A paragraph with no margins specified.</p>
               <p class="ex1">A paragraph with a 2cm top margin.</p>
               <p>A paragraph with no margins specified.</p>
        </body>
    <html>

Önemli not: Bir hücrenin sayfaya ortalanmasını ve yeterli büyüklükte olmasını istiyorsak ideal genişlik ve yükseklik değerleri şunlardır:

**Width:** 600px

**Height:** 300px

Bu gün satır içinde ve style tag’ında CSS komutlarına biraz çalışarak HTML’ye CSS çekme konusuna çok yönlü bakmaya çalıştım. Sadece

*< link href=”style.css” type=”text/css” rel=”stylesheet”/>*

en kullanışlısı diye buna bağlı kalmak ve olaya dar bakmak istemedim.


CSS’de satır içi listelemeye yarayan koda çalışırken geçmiş bilgilerimi harmanlamak istedim.


    li {
        display: inline;
       }


Bu kod display yani göster ve inline yani demek istediği satır içi listeledir.Kaynak olarak çalıştığım www.w3schools.com web sitesinin editöründe çalıştığımda yatay sıralanmış bir menü oluştuğunu gördüm. Bu benim için önemli çünkü menümü yani nav etiketime yazıcağım kodları bu şekilde oluşturacaktım. Ancak ben textlerin altı çizili olsun istemiyordum. Ekran çıktısında textler altı çiziliydi. Önceki CSS çalışmalarımdan text-decoration:none kodunun underline’ı sildiğini hatırladım. Fakat bir sorun oluştu. Ben li etiketine yazdım ve çalışmadı. Sonra text-decoration sayfasına döndüğümde a tagına yazıldığını gördüm. Buradan anladım ki bir text’e işlem yapmak istiyorsak en içteki hangi tag’ın içerisine yazıldıysa o tag’a kod girmeliyiz. Sonuçta listeye girsekde o listenin içinde link belirten a elementi var ve komut o elementi gördüğünde çalışmayacaktır. Düzenlediğim kodlar şunlardır:


    <html>
        <head>
            <style>
                a {
                   text-shadow:1px 2px 5px blue;
                  }
                li {
                   display: inline;
                  }
            </style>
        </head>
        <body>
            <p>Display a list of links as a horizontal menu:</p>
            <ul>
            <li><a style="text-decoration:none" href="/html/default.asp" target="_blank">HTML</a></li>
            <li><a style="text-decoration:none" href="/css/default.asp" target="_blank">CSS</a></li>
            <li><a style="text-decoration:none" href="/js/default.asp" target="_blank">JavaScript</a></li>
            </ul>
        </body>
    </html>

Bu düzenlemelerden sonra linklerde altı çizili görüntü olmayacaktır. Text-shadow ile de textleri blurlama özelliğini kullanıp mavi renk verdim.


Bu şekilde menü oluşturmayı ana hatlarıyla öğrendim. Hücrelerin web sayfasındaki konumuna daha önceden çalışmıştım. Bu bilgilerimi geliştirerek yavaş yavaş bir web sayfası oluşturacağım.
