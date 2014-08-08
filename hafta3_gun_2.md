# Üçüncü Hafta
##2.gün
**05/08/2014**


Bu gün günlerdir yapamadığım halledemediğim gitHub ile gitBook bağlantısını diğer çalışanların yardımıyla çözebildim ve aradaki bağlantıyı kurduk.Git'in çalışma prensibi şudur:


*EDİTÖR'DE YAZILAN KİTAP-------------->KLASÖRE KAYDEDİLİR-------------->SOURCETREE PROGRAMIYLA KLASÖR 'NEW CLONE' SEÇENEĞİ İLE CLONE EDİLİR------------------->GİTHUB'A COMMİT EDİLİR<----------------------->GİTBOOK'LA GİTHUB BAĞLANTISIYLA DEĞİŞİKLİKLER BİRBİRİNDE GÖRÜNÜR*

Önceden kitabımı editöre yazıp gitBook'a publish ederdim. GitHub'da görünmezdi. Şimdi çalışmalarımı ve notlarımı gitHub'a aktaracağım ve gitHub ile gitBook arasındaki bağlantıdan günlüklerim gitBook'da düzgün birşekilde görünecek.Bunu yapmak için öncelikle Sourcetree programını indirdim. Çünkü gitBook editöründe yazdıklarımın kaydedildiği klasörü Sourcetree'de clone edip değişikliklerin burdan görünmesini sağlamam gerekiyordu.

Öncelikle Sourcetree'yi kurdum.Yükleme aşaması biraz sancılıydı çünkü Sourcetree programı, sistemi ve birbiriyle olan bağlantısı zor olan Git notasyonunun bağlantısının olacağı programdı. Kurulduktan sonra new clone seçeneğinden kitabımın kayıt olduğu '_bilgistaj2014' dosyasını clone ettim. Çünkü buradaki dosyalar benim günlüklerim ve Sourcetree'ye clone edilmezse değişiklikleri algılamazdı. Bundan sonra günlüğüme eklediklerim, çıkardıklarım, düzelttiklerim,yaptığım bütün değişiklikler Sourcetree'de clone'ladığım _bilgistaj2014'de branch(şube) ettiğim master bölümünde görünecekti. Değişiklikler programın üst kısmında new clone bölümünün çubuğunda yer alan 'commit' kısmına tıklayarak commit edilir.Kelime anlamı 'teslim etmek' olan commit teslim etmek üzere değişiklikleri alır. Yine commit ve new clone çubuğunda yer alan add/remove butonuyla commitler push edilmek üzere eklenir. Commit edildiğinde aynı çubukta push kısmında commit olanlar birikir. Ben yaptığım değişiklikleri bu işlemlerden geçirdikten sonra push kısmında 2 tane commit gördüm. Programı öğrenmeye çalışırken çalışanlardan yardım alarak ilk 6 günü push etmiştik ancak programın karışıklığından nasıl gerçekleştiğini anlayamadık. Ben öğrenmek için programı kurcalarken 7.ve8. günü de push ettiğimi farkettim. Ancak gitHub'a düştüğü halde gitBook'da görünmüyordu. Sonra bunları düzeltmek için _bilgistaj2014 dosyasını açtım ve editörü artık bu dosyada çalıştırdım. 7.ve8. klasörü başka bir klasöre kopyalayıp diğer günleri bu klasöre aktardım ve editörde çalıştırdım. Daha sonra 7.ve 8. günleri tekrar editöre yazıp kopyaladığımda Sourcetree'de değişikliklerin algılandığını gördüm. Commit edip push ettikten sonra bu problemin ortadan kalktığını gördüm.

Daha sonra başka bir problemi de çözmem gerekiyordu. Gün isimlerini değiştirmek istiyordum. Bunun için editör üzerinde gün isimlerini tek tek rename ettim ve istediğim şekle getirdim. Ancak bir sorun vardı. Çünkü save butonu çalışmıyordu. Yani save butonu sadece içerik değişikliğini algılıyordu. Programı save etmem gerekiyordu. İçerik değiştirip save etmeyi düşündüm o zaman isim değişikliğini algılayabilirdi. Bir tanesinde ufak bir içerik değişikliği yaptım ve save ettikten sonra commit edip push ettim. GitHub'a baktığımda değişiklik göremiyordum ancak gitBook'ta değişiklikler kaydedilmişti. GitHub'da sadece tekrardan eklediğim ve isimlerini o anda değiştirdiğim 7.ve8. günlerin isimleri istediğim gibiydi. Yani 2.hafta gün 2 ve 3.hafta gün 1 şeklindeydiler. GitBook'da değişikliklerin kaydedildiğini görünce diğer günleri de rename ettim ve commit edip push ettim. Bütün değişiklikler artık tam istediğim gibi gitBook'daydı aynı zamanda gitHub'a push ediliyordu. Git notasyonundaki senkronu tamamiyle tutturabilmiş ve asıl amacını şuan çözmüş bulunmaktayım.

Git notasyonu versiyon kontrol sistemini sağlar. Versiyon kontrol sistemi yapılan değişiklikleri hiyerarşik şekilde versiyonlayıp değişikliklerin hangi anda yapıldığını kaydeder ve bunları kayıt altında tutar. Bu şekilde yaptığımız değişiklikleri görüp inceleyebilir aslında beğenmezsek geri dönebiliriz ancak bu geridönüş de farklı bir versiyon şeklinde olur.Çünkü yapılan her değişikliğin sonucu çalışmamızın farklı bir versiyonudur.Ayrıca git programımızda ya da projemizde yaptığımız değişiklikleri hemen günlüğe kaydetmez. Push bölümünde birikmesinin sebebi değişklikleri kontrol edip karar değiştirdikten sonra daha günlüğe eklemeden geri çekebilmektir. Bu sayede tekrardan günlükten silmekle ve tekrardan yazmakla zaman harcamayacağız. Ayrıca yapılan bir değişikliği bi yerde kaydedip sonraki değişikliği bir daha kaydetmek ve bunları tekrardan derleyip kontrol altında tutmaya çalışmanın zorluğunu ortadan kaldırmış ve bunu bizim yerimize kendisi yapar hale gelmiştir. Ayrıca bu işlemler sırasında kaybedilen vakti bize kazandırarak proje çalışmalarında ferahça işlem yapabilmemizi ve kendimizi işimize daha rahat verip vakit derdinden bizi kurtarmıştır.

Bugün git notasyonunu ve gitHub ile gitBook arasındaki ilişkiyi tamamen anladım. HTML çalışmalarım ve CSS araştırmalarım sonraki günlerde devam edecektir.