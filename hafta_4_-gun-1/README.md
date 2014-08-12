# Dördüncü hafta
##1. gün
**11/08/2014**

Bugün CSS'de bir web sayfasında hücre içi ve dışı boşluk bırakmayı, yani etiket içinde komut vererek sayfada boşluk bırakmayı, listeleri, tabloları, metin tiplerini inceledim. Örnek kodlar çektim ve onları karıştırdım. Kendim daha iyi anlamak için bu kodlara ekleme ve çıkarma yaptım. Şimdi bu yaptıklarımı yazacağım.

Öncelikle CSS komutlarıyla websayfasında sayfada kenardan üstten alttan sağdan soldan boşluklar bırakmak için iki tane komutumuz var. Padding ve margin. Padding hücre içi yani etiket içerisine yazdığımız metin, link ya da bir resmin konumunu, etiket içerisinde hücre kenarlarına olan boşlukları ayrlar. Margin ise hücrenin web sayfasının kenarlarına göre boşluğunu ayarlar. Genel açıklaması şudur:

**Padding :**

Padding özelliği hücre içi boşluk vermek için kullanılır.Buradaki hücre tanımı div’i temsil etmektedir.

**Margin:**

Margin elementi hücre dışı boşluk vermede kullanılır.

Eğer margin’e veya padding'e 4 tane pixel örneği verirsek saat yönünde 4 yönde hücre içi ya da hücre dışı boşluk verir.

    div {
        width: 600px;
        height: 300px;
        background-color: goldenrod;
        color: darkslategray;
        font-size: 18px;
        padding: 25px 50px 75px 100px;
       }

Bu kod satırında bu dört sayı saat yönüne göre hesaplanır. 25px padding-top, 50px padding-right, 75px padding-bottom ve 100px padding-left anlamındadır.

Araştırdığım bazı özellikleri liste halinde sıraladım. Bu özellikler şunlardır:

- Border sınır demektir. Eğer hücremize yani divimize sınır vermek istiyorsak border ibaresini kullanırız.
- Line-height satır yüksekliğini ayarlamamız için kullanılır. Buna verdiğimiz bir pixel değeri satırlar arası boşluğu değiştirir.
- Harfler arasında boşluk vermek için letter-spacing kullanılır. Bu özelliğe verdiğimiz değer harfler arasındaki boşluğu değiştirir.
- Text-align metinleri sayfa içinde veya kullanıldıkları element içinde hizalamak için kullanılır.4 çeşit kullanım şekli vardır. Center,left,right,justify.
- Text-shadow metinleri göstermek için kullanılır. Text-shadow’u 5px ayarlarsak blur olur yani metin bulanıklaşır.
- Text-transform önemlidir. Bu özellik metinlerin harflerini belirtir. Özellik capatalize olursa metinlerin ilk harfleri büyük olur. Uparcase bütün harfleri büyük yapar, lowercase bütün harfleri küçük yapar.
- Font metinlerin yazı tipini belirler. Font-family özelliğinde font ailesinin adında birden fazla kelime varsa tırnak içinde belirtilir.

      p {
         font-family: "Times New Roman", Times, serif;
         }

Bir metnin pixelini ayarlamak için font-size özelliğini kullanmalıyız. Çünkü size boyut anlamına gelir.


       P {
           Font-size: 50px;
         }




 #####*Kısa bir html hatırlatması:*
 *Eğer bir link oluşturduktan sonra o link’in istediğimiz web sayfasına yönelmesini istiyorsak <a href=http://ornekwebsite.com target=”_blank”> bu bir linktir</a> görüldüğü gibi ‘target’ ifadesi ile _blank kullanılır. Yani target=”_blank” kullanılır.*


 **CSS listeleri:**

 HTML’de sıralı ve sırasız liste vardır. Sıralı liste için < ol > sırasız liste içinse < ul > etiketi kullanılır. CSS ile bu etiketler için bazı class’lar yazıp listeleri daha farklı hale    getirebiliriz. Listelere tarz verebiliriz. CSS’de listeler için yazılması gereken özellik       ‘list-style-type’ dır.


    <html>
        <head>
            <style>
                ul.a {
                 list-style-type: circle;
                   }
                ul.b {
                 list-style-type: square;
                   }
                ol.c {
                 list-style-type: upper-roman;
                   }
                ol.d {
                 list-style-type: lower-alpha;
                   }
            </style>
        </head>
        <body>
            <p>Example of unordered lists:</p>
                <ul class="a">
                    <li>Coffee</li>
                    <li>Tea</li>
                    <li>Coca Cola</li>
                </ul>
                <ul class="b">
                    <li>Coffee</li>
                    <li>Tea</li>
                    <li>Coca Cola</li>
                </ul>
            <p>Example of ordered lists:</p>
                <ol class="c">
                    <li>Coffee</li>
                    <li>Tea</li>
                    <li>Coca Cola</li>
                </ol>
                <ol class="d">
                    <li>Coffee</li>
                    <li>Tea</li>
                    <li>Coca Cola</li>
                </ol>
        </body>
    </html>

Bu kodu yazdığımızda görüldüğü gibi her class için tanımlanan etiketlerde listelerin çıktısı ekrandadır.


<html>
    <head>
        <style>
            ul.a {
             list-style-type: circle;
               }
            ul.b {
             list-style-type: square;
               }
            ol.c {
             list-style-type: upper-roman;
               }
            ol.d {
             list-style-type: lower-alpha;
               }
        </style>
    </head>
    <body>
        <p>Example of unordered lists:</p>
            <ul class="a">
                <li>Coffee</li>
                <li>Tea</li>
                <li>Coca Cola</li>
            </ul>
            <ul class="b">
                <li>Coffee</li>
                <li>Tea</li>
                <li>Coca Cola</li>
            </ul>
        <p>Example of ordered lists:</p>
            <ol class="c">
                <li>Coffee</li>
                <li>Tea</li>
                <li>Coca Cola</li>
            </ol>
            <ol class="d">
                <li>Coffee</li>
                <li>Tea</li>
                <li>Coca Cola</li>
            </ol>
    </body>
</html>


Listeleri bir resim ya da arka plan görseli şeklinde tutmak istiyorsak arka plana resim koyma özelliği olan background-image: url(“resim.png”) gibi bir syntaxla oluştururuz. List-style-image: url(“resim.png”) hatta syntaxları birbirinin neredeyse aynısıdır.

**Tablo:**

CSS’de tablo oluşumunda table etiketi ile diğer etiketler arasında farklı bir durum vardır. Table yani tablo etiketinin sınırları farklıdır ve bunu durdurmazsak iki tane sınır olacaktır.

    table {
         border-collapse: collapse;
         }
    table, td, th {
         border: 1px solid black;
         }


Bu  kod satırlarında tableyi ayrı bi yerde farklı tanıttıktan sonra diğer özellikler için ayrı bir class açmamızın sebebi table’da sınırları kaldırmak istedik. Border-collapse:collapse; özelliğini kullandık. Collapse kelime anlamı olarak çöküşe yakındır. Yani dış sınırları çökertmiştir. Border da sınır anlamına geldiği için sınır çöküşü anlamı taşımaktadır.Table,td ve th tagları için tek çatı altında ortak özellik yazılacaksa ayrı bi yerde hepsi için CSS kodu yazılabilir.

Daha önce kullandığım basit tablo HTML kodunda etiketlerin içine yazdığım textleri ortalamak için örneğin < td >Ali< td > yi etiket içinde ortalamak için < td align=”center > etiketini kullanırdım. Şimdi ise CSS ile kaynak olarak da kullandığım http://www.w3schools.com/ websitesindeki tablo çalışmasını aldım ve burda < style > tag’ı içine < td > tagındaki text’i ortalaması için

*td
{  text-align: center; }*

tagını yazdım.Böylece her seferinde < td > tagları içerisine aling=”center” kodunu yazmaktan kurtuldum. CSS’in faydalarını kodlarla uğraştıkça zaman içerisinde görmekteyim.

Table td ve th etikerleri eğer ortak CSS özellikleri içerebiliyorsa tek parametrede yazılabilir. Bunu öğrendim ve bu parametrenin içine küçük de olsa kendi align-text:center kodumu yerleştirerek textlerin ortalanmasını sağladım.
Tablo genişliği ve yüksekliğini ayarlamak için width ve height özelliklerini kullanırız. Width genişlik demektir. Height ise yükseklik anlamına gelir.

    Table {
         Width:%100;
         }
    Th
         {
         Height:50px;
          }

Bu kod satırları tablonun genişliğini sayfanın tamamına yayar ve th tagının yüksekliğini de 50 pixel olarak ayarlar.


Bu gün CSS komutlarında tabloları, tabloya resim vermeyi, listelerde arka planı ve ul tagı içine yazdığım listeleri CSS ile ul içine padding komutuyla sağda boşluk bırakmayı öğrendim. İlgili kısa kod satırı şudur:

      ul{
       pading-left:15px
       }
Öğrendiğim bu kısa ve net bilgilerle tabloyla listeyle uğraşırken öğrendiğim en net bilgi CSS'in önemi oldu. Çünkü tablo yazarken CSS olmadan yazdığımda her td tagında textleri ortalamak için center komutu verirdim. Şimdi tek CSS satırıyla bu zahmetten kurtuldum. Kod kalabalığına çözüm bulduğu kadar kafa karışıklığını ve uğraştırıcılığı da ortadan kaldırdığını farkettim.

