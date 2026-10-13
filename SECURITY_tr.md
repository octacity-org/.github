# Güvenlik Politikası

> 🌐 English version: [SECURITY.md](./SECURITY.md).

Octacity projelerinin güvenliğini artırmaya yardımcı olduğunuz için teşekkür ederiz.

Bu belge, organizasyon genelinde kullanılan varsayılan güvenlik bildirimi kurallarını içerir. Repository'ler ek veya farklı gereksinimler tanımlayabilir; bu nedenle önce mutlaka repository'nin kendi `SECURITY.md` dosyasını, README dosyasını ve katkı kurallarını inceleyin.

Repository'ye özel güvenlik politikaları bu belgeden önce gelir.

## Desteklenen Sürümler

Repository aksini belirtmediği sürece güvenlik düzeltmeleri varsayılan branch için sağlanır.

Sorumlu ekipler, repository düzeyindeki güvenlik politikalarında belirli sürümler, branch'ler veya dağıtım ortamları için destek tanımlayabilir.

## Güvenlik Açığı Bildirme

Verileri, yetkileri, gizli bilgileri, sistem erişimini, erişilebilirliği veya kod çalıştırmayı açığa çıkarabilecek ciddiye alınabilir güvenlik açıkları, GitHub Private Vulnerability Reporting üzerinden özel olarak bildirilmelidir.

Etkilenen repository'nin **Security** sekmesini kullanın ve seçenek mevcutsa **Report a vulnerability** seçeneğini seçin.

Kullanıcıları, dağıtımları, maintainer'ları veya altyapıyı riske atabilecek bir güvenlik açığı için herkese açık issue açmayın.

Güvenlik veya emniyet açısından kritik repository'lerin GitHub Private Vulnerability Reporting özelliğini etkinleştirmesi kuvvetle tavsiye edilir.

## Neler Özel Olarak Bildirilmeli

Bir sorun aşağıdakilere olanak tanıyabiliyorsa özel bildirim uygundur:

- Verilere veya hesaplara yetkisiz erişim
- Kimlik doğrulama veya yetkilendirmenin atlatılması
- Kimlik bilgilerinin, token'ların, anahtarların veya diğer gizli bilgilerin açığa çıkması
- Uzaktan veya istenmeyen kod çalıştırma
- Yetki yükseltme
- Enjeksiyon saldırıları
- Güvenlik sınırlarının aşılması
- Güvensiz dosya erişimi veya path traversal
- Ciddi kriptografik yanlış kullanım
- Gerçekçi pratik etkisi olan hizmet engelleme
- Tedarik zinciri ihlali
- Dağıtılmış sistemlerin veya kullanıcıların istismarı

Emin olmadığınızda özel bildirimi tercih edin.

## Neler Herkese Açık Bildirilebilir

Olağan güvenlik iyileştirmeleri, ciddiye alınabilir ve istismar edilebilir bir açığı ortaya çıkarmadığı sürece herkese açık issue'lar üzerinden tartışılabilir.

Örnekler:

- Genel bağımlılık güncellemeleri
- Sıkılaştırma önerileri
- Daha güvenli varsayılanlar
- Ek doğrulama
- Dokümantasyon iyileştirmeleri
- Katmanlı savunma değişiklikleri
- Gerçekçi bir saldırı yolu bulunmayan statik analiz bulguları
- Test, loglama veya izleme iyileştirmeleri
- Gelecekteki güvenlik riskini azaltan yeniden düzenlemeler

Herkese açık tartışma mevcut bir zayıflığın nasıl istismar edileceğini ortaya çıkarabilecekse, bunun yerine özel olarak bildirin.

## Eklenmesi Gereken Bilgiler

Yararlı bir bildirim mümkün olduğunda şunları içermelidir:

- Etkilenen repository, bileşen, branch veya sürüm
- Sorunun net bir açıklaması
- Beklenen güvenlik sınırı
- Gösterilmiş veya olası etki
- Sorunu yeniden üretme adımları
- Asgari bir kavram kanıtı
- İlgili loglar, ekran görüntüleri, istekler veya kod
- İstismar için gereken koşullar
- Biliniyorsa önerilen çözüm

Bildirimler, doğrulanmış davranışı varsayımlardan veya doğrulanmamış olasılıklardan ayırmalıdır.

Gereksiz özel veri, kimlik bilgisi veya gizli bilgi eklemeyin.

## Güvenli ve Zarar Vermeyen Araştırma

Güvenlik testi, sorunu göstermek için gerekli olanla sınırlı tutulmalıdır.

Şunları yapmayın:

- Size ait olmayan verilere erişmek, bunları değiştirmek, silmek veya saklamak
- Yetkisiz erişim gösterildikten sonra özel verileri incelemeye devam etmek
- Hizmetleri aksatmak veya erişilebilirliği düşürmek
- Hizmet engelleme veya yüksek hacimli yük testi yapmak
- Sistemlere veya verilere zarar vermek, bunları bozmak ya da silmek
- Kalıcılık sağlamak
- Zararlı yazılım yerleştirmek
- Sosyal mühendislik, oltalama veya kimliğe bürünme yöntemlerini kullanmak
- Üçüncü taraf altyapısını veya hizmetlerini hedef almak
- Değerlendirme izniniz olmayan sistemler üzerinde test yapmak
- Koordineli açıklamadan önce çalışan istismar ayrıntılarını kamuya açıklamak

Mümkün olduğunca yerel ortamları, test örneklerini, kendi kontrolünüzdeki hesapları ve asgari kavram kanıtlarını kullanın.

Sorunu kanıtlamak için gerekenin ötesinde özel verilerle, kimlik bilgileriyle, gizli bilgilerle veya erişimle beklenmedik biçimde karşılaşırsanız:

1. Testi durdurun.
2. Bilgiyi saklamayın, kopyalamayın, kullanmayın veya paylaşmayın.
3. Durumu derhal GitHub Private Vulnerability Reporting üzerinden bildirin.
4. Neye, nasıl erişildiğini açıklayın.

## Koordineli Açıklama

Bildirimde bulunanlar, sorumlu ekip inceleme yapıp yanıt hazırlarken, ciddiye alınabilir ve kamuya açık olmayan güvenlik açıklarını gizli tutmalıdır.

Kamuya açıklama, sorumlu ekiple koordineli olarak yapılmalıdır.

Octacity süresiz gizlilik talep etmez; ancak bildirimde bulunanların, teknik ayrıntıları yayımlamadan önce inceleme, düzeltme, sürüm hazırlığı ve kullanıcılarla iletişim için makul bir fırsat tanıması beklenir.

Kullanıcıları veya dağıtımları korumak için makul ölçüde ek süre gerektiğinde sorumlu ekip, bildirimde bulunandan açıklamayı ertelemesini isteyebilir.

## İnceleme ve Sorumluluk

Bildirimi ele almak, etkilenen repository'nin sorumlu ekibinin görevidir.

Ekip lideri:

- Bildirimi doğrudan inceleyebilir
- İncelemeyi bir ekip üyesine devredebilir
- Bir repository maintainer'ı atayabilir
- Başka bir Octacity ekibinin yetkin bir üyesinden yardım isteyebilir
- İlgili upstream projeler veya hizmet sağlayıcılarla koordinasyon kurabilir

Bildirimin geçerli olup olmadığına, önem derecesine, uygun çözüme ve açıklama sürecine sorumlu ekip karar verir.

Güvenlik bildirimleri, Octacity [Katkı Kuralları](CONTRIBUTING_tr.md)'nda anlatılan hesap verebilirlik ve inceleme ilkelerine göre ele alınır.

## Yanıt Süreleri

Octacity; alındı bildirimi, inceleme veya düzeltme için sabit süreler garanti etmez.

Yanıt süresi şunlara bağlı olabilir:

- Maintainer'ların müsaitliği
- Proje hareketliliği
- Teknik karmaşıklık
- Önem derecesi ve istismar edilebilirlik
- Etkilenen sistemlere erişim
- Bağımlılıklarla veya dış hizmetlerle koordinasyon

Sorumlu ekipler, makul ölçüde mümkün olduğunda yanıt vermeli ve ilerlemeyi bildirmelidir.

## Yapay Zekâ Destekli ve Otomatik Bildirimler

Yapay zekâ destekli analiz, tarayıcılar, fuzzer'lar ve otomatik araçlar kullanılabilir.

Gönderimin sorumluluğu bildirimde bulunana aittir ve bu kişi:

- Sorunun ciddiye alınabilir olduğunu doğrulamalı
- Bildirilen davranışı anlamalı
- Yararlı bir yeniden üretim yöntemi veya kanıt sunmalı
- Doğrulanmış bulguları üretilmiş spekülasyondan ayırmalı
- Maintainer sorularına bizzat yanıt vermeli
- Doğrulanmamış çıktıyı büyük hacimlerde göndermekten kaçınmalı
- Repository'nin kurallarına ve bu güvenlik politikasına uymalıdır

Octacity, otonom bir ajanla değil, bildirimin sorumlusu olan kişiyle iletişim kurmayı bekler.

Doğrulanmamış tarayıcı çıktıları, spekülatif yapay zekâ üretimi bildirimler ve gerçekçi bir saldırı yolu içermeyen bildirimler daha fazla incelenmeden kapatılabilir.

## Ödüller ve Tanınma

Octacity bir bug bounty programı yürütmez ve belirli bir proje veya program için açıkça duyurulmadıkça maddi ödül sunmaz.

Octacity, geçerli güvenlik açıklarını bildirenlere, anonim kalmak istemedikleri sürece, genellikle GitHub kullanıcı adlarıyla kamuya açık biçimde teşekkür edebilir.

Teşekkür şuralarda yer alabilir:

- Repository sürüm notları
- Güvenlik duyuruları
- Teşekkür dosyaları
- Proje dokümantasyonu
- Organizasyon düzeyinde bir katkıcı listesi

Teşekkürün biçimi ve yeri değişebilir; kamuya açık teşekkür garanti edilmez.

## Gizlilik

GitHub Private Vulnerability Reporting üzerinden gönderilen bilgiler, sorunun incelenmesine ve çözülmesine dahil olan kişilerle sınırlı kalmalıdır.

Bildirimde bulunanlar; özel bildirim içeriğini, maintainer görüşmelerini, yamaları veya istismar ayrıntılarını koordinasyon olmadan paylaşmamalıdır.

Maintainer'lar, bildirimde bulunanın bilgilerini bildirimi ele almak için gerekenin ötesinde paylaşmaktan kaçınmalıdır.

## Kapsam Dışı

Aşağıdakiler, gerçekçi bir güvenlik etkisi göstermedikçe genellikle güvenlik açığı olarak değerlendirilmez:

- İstismar edilebilir bir sonucu olmayan eksik iyi uygulamalar
- İlgili bir saldırı yolu içermeyen bağımlılık sürümü bildirimleri
- Doğrulanmamış otomatik tarama sonuçları
- Kullanıcının kasıtlı olarak kendisine karşı kod çalıştırmasını gerektiren self-XSS
- Tamamen desteklenmeyen veya kasıtlı olarak güvensiz yapılandırmalara dayanan bildirimler
- Sosyal mühendislik
- Fiziksel saldırılar
- Önceden izin alınmadan yapılan hizmet engelleme testleri
- Octacity'nin kontrolü dışındaki üçüncü taraf hizmetlerdeki sorunlar
- Zaten bilinen bir sorunun mükerrer bildirimleri

Sorumlu ekipler repository'ye özel kapsam tanımlayabilir.

## İyi Niyetli Bildirim

Octacity, bu politikaya uyan iyi niyetli güvenlik araştırmalarına değer verir.

Dürüstçe, özenle ve zarar verici ya da yıkıcı davranış olmadan yapılan bildirimler saygıyla incelenir.

Bu politika, sahibi olmadığınız veya değerlendirme izniniz bulunmayan sistemler, hesaplar, altyapı veya veriler üzerinde test yapmaya yetki vermez.

## Sorular

Bir sorunun herkese açık mı yoksa özel mi bildirilmesi gerektiğinden emin değilseniz GitHub Private Vulnerability Reporting kullanın.

Etkilenen repository'de özel güvenlik açığı bildirimi etkin değilse, istismar ayrıntılarını kamuya açıklamadan, mevcut en güvenli proje kanalı üzerinden sorumlu ekiple iletişime geçin.
