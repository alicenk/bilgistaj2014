# Dördüncü hafta
## 5.gün
**15/08/2014**

Bu gün websayfamda z-index kullanımını öğrendim. z-index websayfadaki divleri sıraya koyar.Fakat bütün parametlerelerini de arka plana atar. Yani z-index bir yandan düzenleme işine baksa bile öteki taraftan kullanılması tehlikeli bir parametredir.Bugün web sayfamda devam ettiğim çalışmalarımla beraber yaşadığım z-index problemiyle uğraştım.

Web sayfamda header kısmında değişiklikler yaptım. Arka plan rengini değiştirdim. Form oluşturdum ve formu position değerleri kullanarak header'de sayfanın sağ tarafına aldım. Form oluştururken eski bilgilerimi yeterince pekiştirdim.

Daha sonra sayfama bir arama motoru ekledim. Bu arama motoru websayfasının header kısmında yer almalıydı. Header kısmında bir arama motoru kodladım.

    <label class="arama">ARAMA:</label>
    <input class="arama" type="search" name="googlesearch"/>

Bu kodlarla bir arama motoru head kısmına ekledim. CSS class'ı olmadığı için arama motoru head'ın en altında küçük bi yerde logonun sağında yer alıyordu. CSS class'ı açıp arama motorunun header'daki yerini belirledim.

     .arama{
       position:relative;
       left:230px;
       width:400px;
       font-size:20px;
       font-style:italic;
       text-decoration:bold;
       font-weight:bold;
         }


Kodlarda görüldüğü gibi arama motorunun genişliğini ve label'ındaki text'in size'ını belirledikten sonra aside kısmının ayarlamasına geçtim. Hücreler belirsin diye hepsine bir fieldset çektim çünkü websayfasındaki bölümlerin kapladıkları alanı somut olarak görmem gerekiyordu. Fieldset çektiğimde aside division'un üstünde oluyordu. Position ve padding,margin ayarlarını yapsam da sonuç değişmiyordu. Bende aside'i divin içine aldım.

Bu sırada bir problemle karşılaştım. Daha önce borderlarını belirlediğim ve textlerini mavi renkle blurladığım textlere link vermiştim. Ancak division içindeki aside'de yazdığım paragrafta da link beliriyordu. Aside bölümünü sildim başka text yazdım fakat ona da link veriyodu. Sonra anladığım kadarıyla CSS kodlarında classladığım kırmızı renkli kutucuktaki paragrafı linklerken < a href="örnekwebsite.com" > < /a > etiketinin doğru yazılışı bu olduğu halde ben < a href="örnekwebsite.com" /> şeklinmde yazdığımdan dolayı bu istediğimi yapamadım.

Bu sorunu çözmek için sayfanın kaynak kodlarını gösteren tarayıcı özelliğinde öğeyi denetle butonuna tıkladım. Websayfamdaki bölümlere tek tek baktım inceledim ve uzun uğraş sonucu bu küçük hatayı düzelttim.

Daha sonra aside bölümüne bir takvim eklemek istedim. Bunun için araştırma yapmay başladım ve takvim eklemek için gereken kodun JavaScript'e dahil olduğunu gördüm.

Bu kod javaScript'e başlamama öncü olabilecek diye düşünüyorum.

     <script language="javascript" src="http://in.sitekodlari.com/takvim3.js"></script>


Daha sonra eski HTML bilgilerimden hatırladığım target etiketiyle birlikte siteme sosyal medya düğmelerini eklemek istedim. Websayfasına resim ekleme mantığıyla aynı olan < a href="http://www.facebook.com">< img src="facebooklogosu.png"/>< /a>
etiketini kullandım. Bu etiketle facebook logosuna link vermiş oldum ve kullanıcının her tıkladığımda facebook'a ya da link verdiğim diğer sosyal ağlardan birine yönelicek olmasını sağlamış oldum.

Ancak asıl amacım logolara tıkladığımda websayfamın üzerinden o siteye gitmemesiydi. Yeni bir sayfa olarak o web sayfasına yönelmesiydi. Bunun içinse eski HTML bilgilerimden yararlanıp target=new komutunu kullandım. < a > tagına bu komutu verdiğimde linklediğim websayfasına tıkladığımda o websayfası ayrı bir sayfa olarak açılıyordu. Zaten target kelimesi dilimizde de hedef anlamına gelmektedir.

Bu işlemlerimde kullandığım kod kısmı şudur:


        <a class="sosyalağ1" href="http://www.facebook.com" target=new><img src="http://in.sitekodlari.com/fb/facebook4.png" border="0"></a>
        <a class="sosyalağ2" href="http://twitter.com/" target=new><img src="http://in.sitekodlari.com/tw/21.png" border="0"></a>
        <a class="sosyalağ3" href="http://Instagram.com/" target=new><img src="http://in.sitekodlari.com/insta/8.png" border="0"></a>


Bugünki çalışmamda z-index kullanımını , websayfasına arama motoru eklemeyi , websayfama logo eklemeyi öğrendim. Araştırarak bulduğum ve aside kısmına eklemem gereken basit script kodu olan takvim oluşturma kodunu kullandım.Web sayfama logo ekledim ve CSS'in position özelliğiyle bunların websayfasının header bölümündeki yerini belirledim. Daha önce yaptığım küçük kod hatalarını bulup düzenledim.
