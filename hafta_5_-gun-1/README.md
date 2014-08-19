# Beşinci hafta
##Birinci gün
**18/08/2014**

Bugün çalıştığım kaynak site olan zinzinzibidi.com da ileri CSS konularına geçtim. Tekrar arka plan konusuna derinlemesine değinildi. Bende üzerinden geçtim. Bildiklerim üzerinde durmadım bilmediklerimi öğrenmeye çalıştım. Bu konuda öğrendiğim daha doğrusu zinzinzibidi'nin kaynak olarak gösterdiği bir web site işime çok yaradı.

Geçişli arkaplan özelliği CSS3'de gelmiş bir özelliktir.

http://www.colorzilla.com/

Web sitesinden yararlanarak arka plan rengimi belirledim.Bu websitesi belirlenen arkaplan renginin CSS kodlarını direk olarak çıkarıyor. Bu CSS kodlarını body classıma yerleştirdim.

    body{
        background: rgb(254,191,1); /* Old browsers */
        background: -moz-linear-gradient(top,  rgba(254,191,1,1) 0%, rgba(254,191,1,1) 15%, rgba(254,191,1,1) 33%, rgba(254,191,1,1) 33%, rgba(254,191,1,1) 42%, rgba(254,191,1,1) 56%, rgba(254,191,1,1) 60%, rgba(254,191,1,1) 73%, rgba(254,191,1,1) 76%, rgba(254,191,1,1) 97%); /* FF3.6+ */
        background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,rgba(254,191,1,1)), color-stop(15%,rgba(254,191,1,1)), color-stop(33%,rgba(254,191,1,1)), color-stop(33%,rgba(254,191,1,1)), color-stop(42%,rgba(254,191,1,1)), color-stop(56%,rgba(254,191,1,1)), color-stop(60%,rgba(254,191,1,1)), color-stop(73%,rgba(254,191,1,1)), color-stop(76%,rgba(254,191,1,1)), color-stop(97%,rgba(254,191,1,1))); /* Chrome,Safari4+ */
        background: -webkit-linear-gradient(top,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* Chrome10+,Safari5.1+ */
        background: -o-linear-gradient(top,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* Opera 11.10+ */
        background: -ms-linear-gradient(top,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* IE10+ */
        background: linear-gradient(to bottom,  rgba(254,191,1,1) 0%,rgba(254,191,1,1) 15%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 33%,rgba(254,191,1,1) 42%,rgba(254,191,1,1) 56%,rgba(254,191,1,1) 60%,rgba(254,191,1,1) 73%,rgba(254,191,1,1) 76%,rgba(254,191,1,1) 97%); /* W3C */
        filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#febf01', endColorstr='#febf01',GradientType=0 ); /* IE6-9 */
        }
Görüldüğü gibi oldukça karmaşık ve detaylı. Ancak geçişli arkaplan özelliği için css kodlarıma katmayı tercih ettim.

Logomda değişiklik yapmak istedim. Bunun için hazır logolardan birini kullandım ve < a href > tagına < img src > tagıyla linklediğim önceki logomun yerine yenisinin url'sini kopyaladım.

Bu işlemler sonrasında bugün sözde sınıf olan pseudo class'lara çalıştım. Hover classını kullanarak forumdaki textboxlarıma skyblue rengi verdim. Hover classı sözde sınıfların en çok kullanılan classıdır. Sözde sınıfların syntax'ı şu şekildedir:

    #deneme:hover {
        background-color: violet;
        }

ID'sini tanımladığımız bu deneme sınıfının sözde sınıfı olan hover classına arka plan rengi olarak violet yani eflatun rengi verdiğimde body'min rengi maviden mause'la üstüne geldiğimde eflatuna döndü.

Sözde sınıflar aslında tamamen sınıf olmamalarına rağmen atandığı elemente kalıcı bazı değişiklikler yapar. Ben de hover class'ını kullanarak anasayfamdaki formda kullandığım textboxlara değişiklikler yapmak için bir class tanımladım. Tanımladığım CSS clasları şunlardır:

    .change-color:hover{
         background-color:skyblue;
        }

Form sayfamda < input type="text" > etiketinin aslında bağlı olduğu bir CSS class'ı yoktu. Ben ayrı bi yerde change-color class'ı tanımlamak yerine sözde sınıfla kendi class'ımı bir tanımladım. Bu şekilde mausela textboxların üzerine geldiğimde renkleri gökmavi oldu.

Daha sonra change-color sınıfı oluşturarak skyblue rengini gerçek renkleri olarak ayarladım. Hover sözde sınıfıyla opacity özelliğini keşfedip 0.5 olarak ayarladım. Bu şekilde olduğunda form sayfamdaki textboxların üzerine fareyle gelindiğinde rengi 0.5 oranında saydamlaşıyordu.
İlgili kod satırı:
      #change.color:hover{
         opacity:0.5;
             }


Daha sonra hover özelliğini değiştirip yerine sadece focus yazdım. Bunu yaptığımda elementin üzerine tıklanmadığı sürece hiçbi değişikliği göstermedi.Bu şekilde hover sözde sınıfıyla focus sözde sınıfının arasındaki farkı anladım. Hover sözde sınıfı fareyle üzerine geldiğimizde değişikliği gösterir. Focus ile fareyle tıklamamız gerekir ve başka bi yere fareyi sürüklesek bile değişiklik o elementte kalır.


Bu gün text boxlarımı belirginleştirdim. Butonlarımın üzerinden fareyle geçildiğinde farklı bir renk belirmesini sağladım. Sözde sınıfları öğrendim ve kullandım.
