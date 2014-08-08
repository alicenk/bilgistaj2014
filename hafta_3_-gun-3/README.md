#Üçüncü hafta
##3.gün

**06/08/2014**



Bu gün HTML bilgilerimi biraz daha genişletmek için ileri düzey konulara giriş yaptım. Şuan HTML ile basit bir web sayfası tasarlayıp kodladığım başka bir sayfayla bağlantısını kurabilir , aralarında geçiş sağlayabilirim. Bir form sayfası oluşturup kullanıcı girişi ve şifre isteyen ,  bilgileri sunucuya aktarıcak 'submit' ya da sıfırlayacak 'reset' butonları oluşturabilirim. Checkbox ekleyebilir , bir liste kutusu yapabilirim. Bu ve benzeri daha bir çok işlemi basit bir web sayfası olarak tasarlayabilirim.

Bunların dışında bugün bir web sayfasının genel yapısını öğrendim. Başlığını ,  etiketlerini , web sayfasının bölümlerini...

Basit olarak bir web sayfasının bölümleri şu şekildedir:
- Container
- Header
- Nav
- Content
- Footer


Kodları ise şu şekildedir:

         <div id="container">
              <header>
              </header>
              <nav>
              </nav>
              <div id="content">
              </div>
              <footer>
              </footer>
         </div>

Containet tüm yapısal elementlerimizi içne alan sayfanın kapsayıcısıdır. Header sayfamızın logosu ve dahili arama motoru gibi temel öğelerini içerir.Nav navigation'dan gelir. Yani yol göstericidir. Bunun anlamı bulunduğu sayfadan nereye yönelebileceğini göstermesidir. Bu yüzden header'in tam altında nav bölümü vardır.

Content ise container'in alt başlığı gibidir. Çünkü web sayfamızın içeriğini buraya yazarız.Web sayfasıyla ilgili bütün içerik burada yer alır. Footer ise sayfanın en altında bulunur ve yapım tarihi, telif hakkı gibi ayrıntılı bilgileri;hakkımızda,iletişim gibi bölümleri içerir.


Buraya kadar web sayfasının basit bir taslağı hakkında ilgili bölümlerin ne olduğunu ve neler içermesi gerektiğini öğrendim. Bir web sitesinin bölümlerinin insan vücuduna benzediğini keşfettim. Her birinin ayrı fonksiyonu bir işlevi var ve hepsi kendi etiketi altında yazılır. Bunun sebebi web sayfasını kod karışıklıklarından kurtarmaktır.


Bir web sayfası genel itibariyle bu bölümlerden meydana gelmektedir.Ancak bu bölümler bir web sayfası için tam olarak yeterli sayılmaz. Web sayfasıyla alakalı konuları, kategorileri, içerikleri, takvim, anket gibi nesneleri içericek bir bölüm de gerekir. Ancak bu bölüm olmasa da web sitesi olabilir.


Sayfada reklam görüntüsünü, kategorileri, takvim ve anket gibi nesneleri içeren bu bölümün adı 'aside' dir. Türkçe karşılığı  *yantaraf* olan aside etiketleri içine yazılan kodlar web sayfasının yan tarafındaki bazı belirli sabit içerikleri oluşturacaktır.


Sayfamızın içine makale yerleştirmek içinse < article >
etiketini kullanmalıyız.Article dilimizde makale anlamına gelir.

Toparlıyacak olursak:

- Container
   -   *Tüm yapısal elementleri içine alan, web sayfasının tamamını kapsayan bölümdür.Bütün etiketler container'e dahildir.<div id="contanier> etiketi ile belirtilir.Diğer bütün etiketler bu etiketin içine yazılır. Contanier bu yüzden hepsini kapsamaktadır.*
-   Header
   -   *Sitenin logosu , dahili arama motoru , sosyal medya düğmeleri , ticari sitelerde üye girişi gibi bağlantıların yer aldığı bölümdür.*

- Nav
   - *Sitenin menüsü nav'a yazılır. Nav'ın açılımı 'navigation' dur. Kişinin bulunduğu websayfasın'dan nereye gidebileceğini belirtir.*
- Content
  - *Dilimizde içerik anlamına gelir ve websayfasıyla ilgili bütün içerik burada bulunur.Div etiketine id olarak tanımlanan container'den başka sadece bu etiket vardır. Çünkü içerik belirtir ve ayrı bir div etiketi gerektirir.Ayrıca:*
    - *< article >*
    - *< header >*
    - *< section >*
    - *< footer >*

   *Bu kısımda bulunur.*
- Aside
     - *Web sayfasında kategoriler, anketler, takvimler gibi nesneler bu bölümdedir.*
- Div
   - *Container ve diğer bütün sayfa bölümleri div'e etiket olarak yazılır. Çünkü hepsi kendi bölümünün etiketleridir ve div 'division' kelimesinden gelir. Division türkçede 'bölüm' anlamındadır. Yani div etiketi diğer etiketlerin içerdiği bölümleri içerir. *


Bu gün bir web sayfasının bölümlerinin neler olduğunu ve hangi bölümlerin hangi etiketler içerisine yazılıp kodlandığını öğrendim. HTML'de temel oluşturma çalışmalarımda sonlara doğru yaklaşırken artık yavaş yavaş CSS'e giriş yapacağım.
