# Beşinci hafta
##İkinci gün
**19/08/2014**

Bugün stajımı bitirmeden önceki son günüm olduğundan dolayı bilgilerimi toparladım. Günlüklerimi kontrol edip eksikleri düzenledim.İleri CSS konularına çalışmaya devam ettim. Bunlardan kalan sözde sınıf elementlerini öğrendim ve websayfama kategori yerleştirdim.

Dün :hover, :focus ve :active sözde sınıflarını öğrenmiş ve bunlardan :hover'la :focus'u kendi websayfamda kullanmıştım. Bugün son olarak :first-child ve :last-child sözde sınıflarını inceledim. Örnekleri kendim denedim ve pekiştirdim.

:first-child, bir div içerisindeki ilk elementi seçer ve özelliklerini değiştirir. :last-child ise bir div içeirsindeki son elementi seçer ve özelliklerini değiştirir. Div içerisinde element olmazsa hiçbir özelliği değiştiremezler. Bunu daha iyi anlamak için zinzinzibidi.com'daki editördeki kodları kendim farklı bir websayfası açarak denemek ve deneyerek görmek istedim.

    #deneme7 {
       width: 600px;
       text-align: left;
       }
    #deneme7 p:first-child {
       font-size: 16px;
       font-weight: bold;
       }
    #deneme7 p:last-child {
       font-size: 16px;
       text-decoration: underline;
       }
Deneme7 ID'sine sahip div'imiz içindeki paragraflardan ilk satırın büyük ve kalın yazılmasını istedim. Son satırın ise büyük ve altı çizili olmasını istedim.

    <div id="deneme7">
       <p>Bu ilk satırdır.</p>
       <p>Bu ikinci satırdır.</p>
       <p>Bu üçüncü satırdır.</p>
       <p>Bu dördüncü satırdır.</p>
       <p>Bu beşinci satırdır.</p>
       <p>Bu son satırdır.</p>
    </div>
Bu HTML kodlarıyla CSS dosyasındaki sözde :last-child ve :first-child classlarını kullandığımda divdeki ilk satır :first-child'daki gibi 16px değerinde ve bold tipinde oldu. İkinci satırsa :last-chil'daki gibi 16px değerinde ve bold tipinde oldu.


Daha sonra kendi anasayfamda kategori oluşturmayı araştırdım. Tahmin ettiğim gibi listelerle oluşturuluyordu ancak alt kategoriler link verilerek sayfalarına yönlendiriliyordu ve benim istediğim tam olarak bu değildi ancak aside tarafında yine de bir kategori olsun istedim. Araştırıp kendi kategorimi oluşturdum. Kategorimin HTML kodları şunlardır:

    <ul class="kategori">
        <li><a href="sayfalinki">Ana Kategori 1</a>
            <ul>
                <li><a href="altkategorilinki">Alt Kategori1</a></li>
                <li><a href="altkategorilinki">Alt Kategori2</a></li>
                <li><a href="altkategorilinki">Alt Kategori3</a></li>
            </ul>
        </li>
        <li><a href="sayfalinki">Ana Kategori 2</a>
            <ul>
                <li><a href="altkategorilinki">Kategori 2 alt kategori</a></li>
            </ul>
        </li>
        <li><a href="sayfalinki">Ana Kategori 3</a>
            <ul>
            <li><a href="altkategorilinki">kategori3 alt kategorisi</a></li>
            </ul>
        </li>
        <li><a href="sayfalinki">Ana Kategori 4</a>
            <ul>
                <li><a href="altkategorilinki">kaetgori4 alt kategorisi</a></li>
            </ul>
         </li>
    </ul>


Oluşturduğum kategorinin isimlerini daha sonra websitemdeki planlarıma göre oluşturacağım. Kategorimin CSS kodları ise şunlardır:

    .kategori { margin:0; padding:0; list-style:none; position:relative; top:20px; }
    .kategori li a { display:block; padding:3px; margin:0px; color:#000; position:relative; top:20px;}
    .kategori li ul { display:none; margin:0px; padding:0px; list-style:none;position:relative; top:20px; }
    .kategori li ul a { color:#555;position:relative; top:20px;}

Oluştuduğum kategorilerin alt kategorilerine ulaşamadım. Fare ile tıklandığında alt kategorilerin açılması için gerekli komutları daha sonra araştıracağım.
