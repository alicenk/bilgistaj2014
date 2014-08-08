# Üçüncü hafta
##4.gün
**07/08/2014**

Bugün HTML araştırlamarımın sonuna ulaştım. Tamamen olmasa da başlangıç düzeyinde HTML bilgileri edindim. Bugüne kadar html adına edindiğim , önemli olduğunu düşündüğüm bilgileri kısa kısa bir Word sayfasına not alıp kaydetmişttim. Bunları bu gün genel tekrar olsun diye inceledim ve tekrar günlüğüme yazacağım.


#####*KISA HTML5 NOTLARI:*

- < img src="http://örnekresim.com" alt="çiçek"/>


img resim ekleme elementidir. Web sitelerinin resmi indekslemesi için alt atıfıyla görselin ne olduğu mutlaka yzılmalıdır.

- < strong > etiketi yazıları kalınlaştırmak için kullanılır. Paragraf etiketi olan < p > içine bunu yazarsak yazı kalın olur. < p bu metin normal yazıldı < /p >
< p > < strong > bu metin kalın yazıldı < /strong > < /p >

- < em > ve < i > etiketleri yazıları yatık yazar. Bunlar < p > etiketinin içinde kullanılırsa eğer oaragraflar yatık tipte sayfada görünür.
- < u > etiketi metinlerin altını çizmeye yarar.
- < small > etiketleri yazıları küçük yazar.< big > etiketi yazıları büyük yazar. < p > < small > küçük yazı < /small >< p >
- Yazıları ortalamak için < center > etiketi vardır. Bunun yerine HTML5 CSS3 kullanmayı destekler. Bu özelliği desteklemez.
- Sıralı listeler için < li >< /li > etiketini < ol >< /ol > etiketinin içine , sırasız listeler için < li > < /li > etiketini < ul > < /ul > etiketinin içine yazarız.

######*İleri HTML etiketleri:*

- Buton oluşturmak için yapmamız gereken tek şey < button > etiketini kullanmaktır. < button > bu bir düğmedir. < /button > yazıp derlediğimiz anda buton oluşturmuş oluruz.
- Eğer HTML kodlarıyla bir açıklama yapmak istiyorsak ve bu kodların kendi kodumuzla karışmasını istemiyorsak yapmamız gereken şey < pre > etiketini kullanmak. Bu etiketin içine yazdıpımız hiçbişey HTML kodu olarak derlenmez. Pre'nin anlamı prewiev'dir ve önizleme anlamına gelir.
- Bir cümleyi veya kelimeyi fosforlu olarak belirtmek istiyorsak o cümleyi veya kelimeyi < mark > etiketi içine yazmalıyız.
- Formda başlık olarak girmek istediğimiz ifadeyi < label > etiketi içine yazabiliriz. Daha sonra < input type = "text" value "cinsiyet"/> ile bir textbox açıp bilgilerimizi o label ile alakalı girebiliriz.
- Butonlar girilen bilgileri, görevleri sunucuya taşır. Bu sebepten ötürü tipleri belirlenmelidir. Yani gönderme butonuysa submit olmalıdır. Onaylamaysa button olmalıdır kendi adı gibi. Bunu belirleyici yapabilmek için türkçe anlamı değer olan value atfıyla tırnak içinde gerekli bilgisini yazarız.Örneğin gönderme butonu yazarken < input type = "submit" value = "gönder" /> yaparız. Value yapmasaydık buton'un üzerinde kendi değeri ya da ismi olmaz submit görevi yazardı.
- Bir form sayfasına kullanıcı adı,girişi olan text kutusu, sunucuya verileri göndermeye yarayan mesaj kutusu da konulabilir. Şöyle ki:
         <label> Mesajınız: </label><textarea rows="2" cols="18"></textarea>
Kod satırıyla mesaj kutusu açılabilir. Row satır demektir. Satır bilgisi burdan verilir. Cols dolaylı olarak sütun demektir. Bu ayarlamalarla mesaj kutusunun limitleri ayarlanır.
- Eğer seçin kutusu oluşturmak istiyorsak kullanacağımız etiket < select > etiketidir. Bu seleck etiketi içinde < option > etiketi içine seçilecek elemanları her biri için ayrı ayrı < option > etiketi içine alınacak şekilde yazarak oluştururuz.



*Genel tekrarımın sonucu olarak derlediğim ve tekrar edip daha iyi kavradığım temel HTML bilgileri bunlardır. Bugün bu HTML bilgilerini daha iyi kavradım ve CSS çalışmalarıma başladığımda bu kodlara CSS kodlarını da ekleyip birlikte çalıştırarak hem HTML hem CSS egzersizi yapmış olacağım.

Bu gün HTML tekrarından sonra biraz daha zamanım kaldığı için biraz CSS araştırmaya başladım. CSS'in daha önce 4 şekilde HTML kodları arasına çağırılabildiğini ve CSS'in sadece < head >< /head > etiketleri arasına yazıldığını araştırmış ve ön bilgi sahibi olmuştum.Bu gün bunları biraz daha irdeledim.

CSS kodları elle HTML kodları arasına yazılmak isteniyorsa < head > etiketi içine < style > elementiyle yazılmalıdır.Yani < head > < style > < /style > < /head> düzeniyle yazılmalıdır ve CSS stilleri şu kurala uyularak yazılır:

Eleman-tanımlayıcı {özellik;değeri;özellik;değeri;...}

Bir de CSS'i başka dosyaya kaydediğ çağırmanın en çok kullanılan yönteminin < link > yöntemi olduğunu öğrendim.

Bknz:

          <head>
             <link rel= “stylesheet”   type=”text/css”    href=”dosya.css”/>
         <head>

Sonraki günlerde CSS'i daha iyi kavrayıp taslak çalışmalarımda uygulayacağım. Bilgilerimi yeterli gördüğümde projemi oluşturmaya başlayacağım.
