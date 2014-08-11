# İkinci Hafta

##1.gün
**04/08/2014**


Bu gün projem için sayfalar arası geçişlerin hangi etiketlerle olabileceğini araştırdım. Kişiden kullanıcı adı ve şifre istendiğinde,bir link'e tıkladığı zaman websitenin içerisinde başka bir sayfaya geçmek için gerekli etiketleri ve kodlamaları öğrendim.Ayrıca bi tane açık kaynaklı twitter clone sitesi keşfettim ve kaynak kodlarını inceledim. Öğrendiklerime benzer kodlama var mı yok mu onu kontrol ettim ve @port ile css dosyası çekme yöntemini kullandıklarını farkettim.


Sayfalar arası geçiş yapmak için öncelikle elimde olan bazı çerez kodları kullandım. Sayfalar arası nasıl geçiş yapıldığını araştırdım ve bir sayfadan ötekine geçiş yapmak için genelde < a >< /a > etiketinin kullanıldığını gördüm. Öncelikle araştırmamla bulduğum basit hazır bir kodu aldım. O kodlar şudur:

    <html>
    		<head>
    		 <title>Link Uygulaması</title>
    		</head>

    	<body>
           <a name="start"></a>
    		<ul>
    		  <li><a href="anasayfa.html">Anasayfa</li></a>
    		  <li><a href="başkanınsayfası.html">Başkanın Sayfası</li></a>
    		  <li><a href="iletişim.html">İletişim</li></a>
    		</ul>
    		  <h1>Anasayfa</h1>
              <p><a href="#end">Sayfa Sonu</a></p>
    		  <hr/><a href="http://www.w3schools.com">
    		  <img src="real madrid.jpg"/>
              </a>
    		  <br/>
              <a href="http://www.wordpress.com">
    		     <img src="Villarreal.png"/>
              </a>
              <a name="end"></a>
              <p><a href="#start">Sayfa Başı</a></p>
    	</body>
    </html>

Bu kod sayfasında sayfalar arası geçiş < li > < /li > etiketleri arasında < a > < /a > etiketleriyle link vererek sağlanmıştır. Bunun içinse yönlendirilecek sayfanın html uzantısıyla link olarak verilmiştir.Sayfa adresi de verilebilirdi.Ancak kodlanırken domain oluşmadığı için sayfalar arasında geçiş sağlamak için html uzantısı gereklidir.

Sayfalar arası geçişi sağlamak için gerekli kod satırları şunlardır:

            <ul>
    		   <li><a href="anasayfa.html">Anasayfa</li></a>
    		   <li><a href="başkanınsayfası.html">Başkanın Sayfası</li></a>
    		   <li><a href="iletişim.html">İletişim</li></a>
    		</ul>


Bu kod satırlarında görüldüğü üzere link uygulaması isimli sayfadan anasayfaya geçiş yapabilmek için anasayfa isimli bir web sayfası olmalı ve html uzantısıyla kaydedilmiş olmalıdır. Yani açıkça html ile kodlanmış bir anasayfa tasarımı olmalıdır. Ben bunun için önceki çalışmalarımda edindiğim form sayfasını kullandım. Form sayfasının kodları şunlardır:


    <html>
       <body bgcolor="yellow">
         <form class="form-horizontal">
    	   <div class="control-group">
    	     <label class="control-label" for="inputEmail">Email</label>
    	   <div class="controls">
    	     <input type="text" id="inputEmail" placeholder="Email"/>
    	   </div>
    	   </div>
    	   <div class="control-group">
    	     <label class="control-label" for="inputPassword">Password</label>
    	  <div class="controls">
    	     <input type="password" id="inputPassword" placeholder="Password">
    	  </div>
     	  </div>
    	  <div class="control-group">
    	  <div class="controls">
    	     <label class="checkbox">
    	       <input type="checkbox"> Remember me
    	     </label>
    	     <button type="submit" class="btn"><a href="deneme.html">Sign in</a></button>
    	   </div>
    	  </div>
        </form>
      </body>
    </html>

Görüldüğü üzere önceki araştırmalarımda edindiğim form sayfasının kaynak kodları bunlardır. Bu kodları notepad++'da .html uzantısıyla anasayfa adında kaydettiğimde artık anasayfa.html isimli bir websayfası oldu. Şimdi link uygulaması başlıklı websayfasındaki anasayfa linkine tıkladığımızda anasayfa.html uzantısıyla kaydettiğimiz form sayfasına yönlendirildik.

Ben biraz daha kodlarla oynamak istedim. Sonuçta e-posta ve şifre girdikten sonra sing in butonu ile sisteme giriş yapılmak üzere tasarlanmış bir form sayfası durumundadır bu web sayfası. Ben form sayfasının kodlarında butonu yöneten kod satırında < a > < /a > etiketi ile link uygulaması başlıklı sayfanın .html uzantısını link olarak tanımladım. İlgili kod satırı şudur:


    <button type="submit" class="btn"><a href="deneme.html">Sign in</a></button>

Görüldüğü üzere bu kod satırında < a > < /a > etiketi olmadığında boş bir buton vardı orda. Ancak < button > < / button > etiketi içine deneme.html'yi link olarak verdiğimde artık o buton boş olmayıp aynı zamanda anasayfaya tıklayıp geldiğimiz yani link uygulaması başlıklı sayfaya geri dönücektir çünkü link uygulamasının .html uzantılı ismini yani denee.html'i link olarak butona tanımladım. Kodlarla oynayıp sayfalar arası geçişlerin nasıl sağlanacağını bu şekilde öğrendim.

Sayfalar arası geçişleri de öğrendikten sonra twitter benzeri açık kaynak kodlu web sayfalarını araştırıp biraz fikir sahibi olmaya çalıştım. Araştırmalarım sonucu [http://twatter.com](http://twatter.com) isimki bir twitter clone'u açık kaynak bir web sitesine rastladım. Kaynak kodlarını kontrol edip incelemeye çalıştım. Bilgidiğim , öğrendiğim birşeylere rastlamaya çalıştım ve 4.gün araştırıp öğrendiğim CSS kodlarının HTML'ye çekilmesinde kullanılan yöntemlerden @import yönteminin benzer bir şekilde kullanıldığını gördüm.


    <style type=​"text/​css" media=​"screen,projection">
        @import url(http://static.ning.com/socialnetworkmain/widgets/index/css/common.min.css?xn_version=2728956736);@import url(http://static.ning.com/socialnetworkmain/widgets/index/css/component.min.css?xn_version=295185491);
    </style>

Bu ve benzeri şekilde birçok css dosyası @import yöntemiyle çağırılıp websayfasında komutları kullanılmıştır. Bu açık kaynak kodlardan ben de web sitemi oluştururken yardım alacağım.
