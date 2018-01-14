# Mobil Uygulamarda Güvenlik Analiz Sistemi

Günlük hayatın önemli bir parçası haline gelen akıllı telefonlar, gün geçtikçe artan yetenekleri ve genişleyen
özellikleri sayesinde bilgisayar sistemlerinin yerini almaya başlamıştır. Geliştirilen uygulamalar sayesinde
günümüzdeki kullanımı fotoğraf makinesinden, navigasyon cihazına, hesap makinesinden, sağlık uygulamalarına
kadar birçok farklı alanda birinci sırada yerini almaktadır. Teknolojik gelişmeler ile mobil cihazların maliyetlerinin
düşmesi bu cihazlara erişimi de kolaylaştırmıştır. Akıllı telefonların kullanımının yaygınlaşması ile birlikte geliştirilen
uygulamaların sayısı da artmış, ancak zararlı uygulamaların sayısında daha da büyük bir artış gözlenmiştir.



Saldırganlar tarafından mobil cihazlara yönelik olarak gerçekleştirilen saldırılardan biri de mobil uygulamaların
içerisine zararlı yazılımların enjekte edilmesidir [1]. Mobil cihazlara bulaşan söz konusu zararlı yazılımlar tüm rehber
bilgisini ele geçirebilmekte, kullanıcıya ait mesajları okuyabilmekte, resim, video ve ses gibi multimedya dosyalarına
erişebilmekte ve kullanıcıya ait konum bilgisini saldırganlara iletebilmektedir. Ayrıca sisteme bulaşmış olan zararlı
yazılımlar, sahip oldukları yeteneklere göre; telefon görüşmelerini anlık olarak dinleme, kullanıcının bulunduğu
ortamın dinlemesi, internet aktivitelerinin takip edilmesi gibi işlemleri gerçekleştirebilmektedir [1].
Zararlı yazılımlara 1970’lerden itibaren rastlanmaya başlanmasına rağmen 2004’te mobil dünyaya girmiştir.
Kaydedilmiş ilk mobil zararlı yazılım olan Cabir Nokia 6600, N-Gage, Panasonic X700 ve Siemens SX1 gibi
bluetooth’u açık cihazlar üzerinden yayılmaya başlamıştır. Bu solucan, zararsız olmasına rağmen telefona girdikten
sonra ekranda ‘Caribe’ metni çıkarıyordu. Sonrasında ise yakınındaki bluetooth’u açık olan herhangi bir cihaza
sıçrayarak yayılıyordu. Mobil sistemlerin gelişimi ile bu zararlı yazılımlar artış göstermiştir ve 2010 yılında Android
platformu için ilk zararlı yazılım ortaya çıkmıştır. ’FakePlayer’ isimli bu yazılım, Rusya’daki özel tarifeli numaralara
pahalı SMS’ler gönderiyordu. 2016 yılında ise ‘Pokemon Go’ ile bir çok sahte uygulamayla birlikte ‘adware’ gibi
zararlı yazılımlar yayılmıştır.



Bu denli artan güvenlik açığı sorunu günümüz mobil uygulamalarında büyük bir risk haline gelmiştir. Geliştirilmesi
planlanan sistem ile bu risklerin son kullanıcıya raporlanması ve uygulamalar kullanılmadan önce bu risklerin test
edebileceği bir ortam oluşturulması hedeflenmektedir. Bu işlem ise mobil uygulama güvenlik analizlerinde kullanılan
dinamik analiz metodu ile gerçekleştirilecektir. Bu analiz yönteminin kullanılmasının sebebi ise; statik analiz
metodunun aksine çalışan uygulamaların yaptıkları sistem çağrılarının, ağ trafiğinin, bellek kullanımının ve işlemci
kullanımının analiz edilebilmesidir ve kod karıştırma gibi tekniklere karşı işlevsel olmasıdır. Çalışmamızın özgün
değeri ise, geliştiricilerden çok son kullanıcılara hitap edecek olmasıdır. Bu amaç doğrultusunda dinamik analiz
metodları kullanılarak kullanıcıya basit bir arayüz ile uygulamaların güvenlik analizi raporları sunulması
hedeflenmektedir. Ulusal güvenliğin öneminin her gecen gün arttığı bir dönemde, çoğu yabancı kaynaklı olan zararlı
yazılımların tespit edilmesi için yapılacak olan milli projenin, ülkemizde bu alandaki açığı kapatarak katkı sağlanması
amaçlanmıştır.
Sistemin mimari yapısı aşağıdaki gibi tasarlanmıştır.

![mobilanalizmimari](https://user-images.githubusercontent.com/26030084/34914485-b63e5b44-f924-11e7-9159-673ac98a881b.PNG)
