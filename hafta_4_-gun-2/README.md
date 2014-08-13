#Dördüncü hafta
##2.gün
**12/08/2014**

Bu gün CSS'de border konusunu öğrendim. Bunu öğrenirken sayfada konum belirleyen padding ve margin özelliklerini iyice pekiştirdim. Border'ın türkçede sınır anlamına geldiğini öğrendim. Bu konuyu araştırırken öğrendiklerimi geçmişte çalıştığım bazı konularla da harmanlayarak bilgilerimi pekiştirdim ve çok basit bir anasayfa tasarladım. Bunları yaparken web sayfasının bölümlerini pekiştirmeye başladım. Bir web sayfasının body bölümünde bir div tanımlayarak sınır değerlerini bu div'de belirttim. Daha sonra div'in konumunu değiştirmek isteyecektim. Body'de tanımlasaydım her etiket için ayrı konum özelliği yazmam gerekecekti. Bu yüzden web sayfasının tasarımını yaparken bölümlerinin de önemini kavradım ve hücrelerle yani bölümlerle işlem yapmaya başladım.

Öncelikle editöründen yararlandığım www.w3schools.com web sitesinde çalışırken border adına gördüğüm bir paragrafı kendi notepad++ editörüme yazarak oradaki örneği bire bir kendim çalışarak pekiştirdim. Daha sonra bu çerçeveyi ortalamak istedim ve CSS kodlarına < center > etiketini yerleştirmek istedim. Yani align-text:center özelliğini yazdığımda ortalanmasını düşündüğümde ortalanmadı. Daha sonra border özellini yazdığım div'e center belirledim ancak olmadı.Bu problemi çözmek için kaynak aldığım editörde font bilgilerine girdim ve text özelliklerini inceledim. Kendim text-align:center özelliğini denediğimde komik karşılanabilecek bir hatamı farkettim. Yazım yanlışı yaptığımdan dolayı textleri ortalayamıyordum.

Bir önceki tablo çalışmamda da textleri ortalayamamıştım. Çünkü satır içi style tanımlarımda align="center" yazmam gerekiyordu. Bunu her satırda yapmam gerekliydi ancak ben style.css uzantılı bir css dosyası oluşturup her tag için align-text:center özelliği yaptım ancak yaptığım yazım yanlışından dolayı istediğim görüntüyü elde edememiştim. Bu yanlışımı bir önceki günlüğümde de düzeltip hatamı telafi ettim. Düzelttiğim kodlar şunlardır:

    <style>
        table, td, th {
              border: 1px solid black;
	          text-align:center;
               }
        table {
              width: 100%;
              }
        th {
              height: 50px;
             }
    </style>

Diğer kodlar gereksiz olduğundan yazmak istemedim. Sadece CSS kodlarının bulunduğu style tag'ında düzeltme yaptığım için kodlamanın geri kalan kısmı gereksizdir. Görüldüğü gibi burada da tabloya sınır verilmiştir.

5.haftadaki tablo çalışmamda ise CSS hakkında neredeyse hiç bilgi sahibi olmadığım için satır içi style tanımlarını yazarken yanlışlık yaptığımdan istediğim çıktıyı alamıyordum. Yani < td align center> Ali < /td> gibi style tanımı yaparak yanlışa düşüyordum. Formata uyarladım ve hatamı orda da telafi ettim.


Daha sonra border hakkında araştırmaya devam ettim. Edindiğim bilgiler üzerine w3schools editöründen edindiğim kısa paragraf kodları üzerinde sınır çalışmaları yapmaya başladım. Edindiğim bilgilere değinmek istiyorum:

**CSS'de border:**


CSS’de border elementlerimize sınır vermek için kullanılır.Sınırı border-style özelliği ile belirleriz.

    P {border-style:solid;}

Kod satırıyla border-style özelliği ile sınırı belirledik.Border-style öncü niteliktedir. Yani diğer sınır özelliklerinin etkisi olmasını istiyorsak önce border-style özelliğini ayarlamamız gerekir. Aksi taktirde diğer sınır özelliklerinin bir etkisi olmayacaktır.Çünkü border-style zaten sınır stili anlamına gelmektedir ve sınırın stilini belirlemezsek o stilin özelliklerini de belirleyemeyiz.


Fakat steno özelliği ile border özelliğinin değerlerini tek çatı altında toplayabiliriz fakat style'ini belirtmeliyiz.

Solid kalın ve sert gibi bir anlama denk gelmektedir. Bu değer sınırın stilini belirtir.

Solidden başka dotted dışında double, dashed, groove gibi birkaç stil daha vardır.

Border'ları oval yapmak içinse border-radius özelliği kullanılır. Öteki türlü özelliğe sınır verirdik Yani border:dotted gibi. Ancak şimdi sınır stili kendisi bir özelliktir ve border-radius'tur.

Border çalışmalarımda öncelikle çalıştığım kaynakların border'ı body içinde değil de bir hücre yani div içerisinde çağırdığını gördüm. Bu yüzden ben de bir hücre belirledim.Ancak herhangi bir etiket için de border belirleyebilirdim fakat amacım bir form sayfası yaratmaktı. Bunun için bir web sayfasının bölümleri üzerinden gitmeli ve o bölümlerin tagları üzerinden çalışmalıydım.


Sınırlarımı belirlemeden önce CSS'de bir center sınıfı oluşturdum. Buradan align-text:center edip textleri ortalamaya ve renk vermeye çalıştım. Bu konuda yaşadığım problemler oldu. Araştırarak çözdüm ve textleri ortalayabildim.

Daha sonra bir div etiketi tanımlayarak bu paragrafları div etiketinin içine yerleştirdim. Div'in style.css dosyasındaki .center sınıfındaki özelliklere erişebilmesi için parametre olarak class="center" tanımlayarak div'i .center CSS sınırına bağladım.

    .center {
        text-align: center;
        color: black;
	 }
Mevzibahis center sınıfı budur. Artık divde yapılan her işlem için bu sınıfın özellikleri geçerli olacaktır. Yani textler div hücresinin ortasında olacak ve renkleri siyah olacak.

Daha sonra div'e ait bir sınıf oluşturdum. Bütün taglar div içinde olduğundan border,padding,margin özelliklerimi div içerisinde tanımlayarak bütün taglar için ortak bir görünüm yaratmaya çalıştım.

Bunu yaparken background'dan yararlandım ve arka plan rengini araştırdığım ve gözüme güzel görünen bir renkin kodunu vererek ayarladım. Daha sonra hücrenin arka planına bir resim yerleştirmek istedim. Bunun için de background-image özelliğini kullandım ve resmin url'sini verdim. Daha sonra no-rapeat özelliğini unuttuğumdan dolayı resmin birden çok çıktısı oldu. No-repeat özelliğini de kullandım fakat resim sol üstte ve kötü görünüyordu. Bu konuya daha sonra değinmek üzere resmi sildim çünkü şuanki amacım div hücresini websayfasında istediğim bir konuma yerleştirmekti. Bu yüzden bir önceki arka plan rengini geri getirdim ve hücre içi-dışı boşlukları ayarlamak için padding ve margin özelliklerini ayarlamaya geçtim.


Padding hücre içi boşluk, margin ise hücre dışı boşluk anlamına gelir. Önce padding'i ayarlamak istedim çünkü hücre dışı boşluk daha önemliydi ve ayarlanması daha zordu. Padding ve margin özelliklerinin alt özelliklerine de değerler vermek gerekiyordu. Soldan boşluk istiyorsak padding-left veya margin-left özelliklerine belirli bir pixel değer girmek gerekiyordu, üstten boşluk istiyorsak padding-top veya margin-top özelliklerine bir pixel değeri vermek gerekiyordu.

Padding'in bir özelliğini geçtiğimiz gün öğrenmişti. Pixel değerlerini saat yönünde girdiğimizde dört bir yandan boşluk bırakıyordu. Bunun için yine steno özelliğinden faydalanmak gerekiyordu. Denedim ancak sonuç alamadım. Bunu da daha sonraki çalışmalarıma araştırmak üzere bıraktım.

Bu güne kadar align özelliğinin hep text alt özelliğini kullanmıştım. Bugün align için de steno özelliğini uygulamak istedim. Div class'ında align:center; komutunu yazdığımda istediğim gibi sınırımın içinde olan div hücresi ortalanmıyordu. Bunu da sonraki çalışmalarımda araştırmak üzere bıraktım.

Padding'e gerekli değerleri girdikten sonra en uygun sonucu steno özelliğiyle 15px değer vererek aldım. Border-style'i *solid black* yaptım.Sınırımın oval olmasını istedim ve bunun üzerine border'ın oval olmasına yarayan border-radius özelliğine 200px değeri deneyerek en uygun olduğuna karar verdim.

Margin-left ve margin-top özelliklerine değer vererek div hücremi sayfanın ortasına getirdim. Margin-left:325px ve margin-top:100px değerlerini girdim.

Artık div hücrem web sayfasında istediğim konumdaydı. Ancak bir button, textbox ve messagebox da tanımlayarak basit bir form çerçevesi yaratmak istedim. Labellardan yararlanıp textboxlara isim verdim.Bunu yaparken eski çalışmalarıma döndüm ve hatırlamadığım bilgilerimi pekiştirdim. Bu bilgiler şunlardır:
-   Textbox oluşturmak için < input > tag'ını kullanırız. Value o metin kutusunun görüntüsünü, değerini, adını gösterir.
-   Textboxların başına < label > etiketleri içine gerekli bilgileri girerek tanımlarız.
-   Messagebox oluşturmak için < textarea > etiketini kullanırız ve rows yani satırlara ve cols yani sütunlara değer girerek istediğimiz kapasitede messagebox oluştururuz.
-   Buton oluşturmak için < button >< /button > etiketleri arasına isim girerek oluştururuz. İnput tag'ıyla da oluşturabiliriz ancak buton kendi classları için daha kullanışlıdır.

Bu bilgilerle basit bir form oluşturdum. Bu güne kadar CSS çalışmalarımda hep web sayfasının background'una renk veya resim vermiştim. Şimdi kendim butonun rengini değiştirmek istedim ve style.css dosyasında buton'un value'si olan gönder isimli bir class oluşturup background-color'a black ve text rengine color'a white vererek siyah renkli beyaz yazılı farklı bir buton oluşturabildim.


Bütün bunlardan farkına vardım ve sonra div hücrem beyaz bir fonda duruyordu. Body'e arka plan resmi yerleştirmek istedim ve bir arka plan resmi bulup url'siyle background-image: özelliğine resmin url'sini vererek arka olan resmini oluşturdum. Artık taslak form sayfam istediğim gibiydi.

Oluşturduğum taslak form sayfasının HTML kodları şunlardır:

    <html>
        <head>
            <title> CSS calismasi</title>
            <link href="style.css" type="text/css" rel="stylesheet"/>
        </head>
        <div class="center">
            <header class="center"><p><b>BU SATIR ANASAYFANIN BASLIGI</b></p></header>
            <h1 class="center">bu satir bir ic baslik</h1>
            <p class="center">Bu paragraf ortalandi ve rengi siyah</p>
            <label>kullanici hesabi<label>
            <input type="text" value="e-mail"/>
            <label class="control-label" for="inputPassword">password</label>
            <input type="controls" value="password">
            <br/>
            <label>message:</label>
            <textarea rows="1" cols="18"></textarea>
          <button class="gonder">Giris Yap</button>
      </div>
    </html>

Oluşturduğum taslak form sayfasının CSS kodları şunlardır:

    .center {
        text-align: center;
        color: black;
	        }
    div{
        width:600px;
        background:#827B60 no-repeat top;
        color:darkslategray;
        font-size:18px;
        padding:15px;
	    margin-left:325px;
        border:10px solid black;
	    border-radius:200px;
    	margin-top:100px;
     }
    .gonder{
        color:white;
	    background-color:black;
	      }
     body{
     background-image:url("http://t2.gstatic.com/images?q=tbn:ANd9GcReyLYp8qVpeTQAsRKkDoYl7JzrB1zrvi4EEormN83wfYKi-GG6Lg");
         }


CSS dosyasında çok fazla kod olmadığı halde link yöntemiyle çekmek istedim. Çünkü link yöntemine alışmam gerektiğini düşündüm. Çünkü daha sonraki çalışmalarımda çok kalabalık CSS stilleri yazmam gerekecek. Şimdiden link yöntemine alışmalıyım ki ilerde kolaylık çekeyim diye düşündüm.

Bugünki çalışmamda CSS'in en önemli özelliklerinden birini daha kavradım. Bir proje üzerinde çalışırken birden fazla etiket için veya bir etiketin birden fazla özelliği için tek CSS class'ı yetebiliyor. Bu çok büyük bir avantaj.
