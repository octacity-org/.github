# Octacity'ye Katkıda Bulunmak

> 🌐 English version: [CONTRIBUTING.md](./CONTRIBUTING.md).

Octacity'ye katkıda bulunmak istediğiniz için teşekkür ederiz.

Bu belge, organizasyon genelinde kullanılan varsayılan katkı kurallarını içerir. Repository'ler ek veya farklı gereksinimler tanımlayabilir; bu nedenle çalışmaya başlamadan önce repository'nin README dosyasını, katkı kurallarını, issue şablonlarını ve pull request şablonunu mutlaka okuyun.

Repository'ye özel kurallar bu belgeden önce gelir.

## Kimler Katkıda Bulunabilir

Aşağıdaki iki gruptan da katkı bekliyoruz:

- Octacity üyeleri
- Organizasyon dışından katkıda bulunanlar

Dışarıdan katkı kabul eden repository'lere katkıda bulunmak için üyelik gerekmez.

Her repository, dışarıdan katkıya şu anda açık olup olmadığını belirtmelidir.

## Dil

Octacity GitHub organizasyonunun çalışma dili İngilizcedir.

Issue'lar, pull request'ler, incelemeler, tartışmalar, üyelik başvuruları, proje önerileri ve projeyle ilgili diğer iletişim İngilizce yazılmalıdır.

Açık ve anlaşılır iletişim beklenir; ancak kusursuz dil bilgisi veya akıcılık şart değildir. Katkıda bulunanlar çeviri veya yazım desteği araçlarını kullanabilir.

Ağırlıklı olarak başka bir dilde yazılmış içeriğin İngilizce olarak yeniden yazılması istenebilir. Güncellenmezse kapatılabilir veya incelenmeden bırakılabilir.

## Başlamadan Önce

Herhangi bir katkıya başlamadan önce bir issue açın.

Issue şunları açıklamalıdır:

- Neyi değiştirmek istediğiniz
- Değişikliğin neden faydalı olduğu
- İzlemeyi düşündüğünüz genel yaklaşım
- Değerlendirdiğiniz alternatifler veya emin olmadığınız noktalar

Bu, sorumlu ekibe bağlam sağlama, çalışmanın uygun olduğunu doğrulama ve tekrarlanan ya da çakışan emeği önleme fırsatı verir.

Bariz yazım hatası düzeltmeleri gibi küçük değişiklikler için repository daha hafif bir süreç tanımlayabilir.

## Bir Issue'yu Üstlenmek

Mevcut bir issue üzerinde çalışmayı düşündüğünüzde şuna benzer bir yorum bırakmanız önerilir:

> I would like to work on this.

Onay beklemeniz kuvvetle tavsiye edilir. Başka biri aynı sorun üzerinde zaten çalışıyor olabilir veya sorumlu ekibin henüz belgelenmemiş ek bilgisi olabilir.

Repository aksini belirtmediği sürece bir issue'yu üstlenmek her yerde zorunlu değildir. Ancak iletişim kurmadan çalışmaya başlayanlar şu riskleri kabul etmiş olur:

- Aynı iş zaten yürütülüyor olabilir
- Önerilen yaklaşım projenin yönüyle çelişebilir
- Katkıya artık ihtiyaç kalmamış olabilir
- İnceleme sırasında kapsamlı değişiklikler istenebilir
- Harcanan emeğe rağmen pull request reddedilebilir

Uygulamaya geçmeden önce iletişim kurmak, herkes için boşa giden emeği önler.

## Mimari ve Önemli Değişiklikler

Mimari değişiklikler uygulanmadan önce tartışılmalıdır.

Aşağıdakileri önemli ölçüde etkileyen değişiklikleri yapmadan önce bir issue açın ve onay bekleyin:

- Proje mimarisi
- Herkese açık API'ler
- Veri formatları veya depolama
- Güvenlik sınırları
- Bağımlılıklar
- Derleme veya dağıtım sistemleri
- Repository yapısı
- Kullanıcıya dönük önemli davranışlar
- Uyumluluk veya geçiş gereksinimleri

Talep edilmemiş büyük yeniden yazımlar göndermeyin.

Sorumlu ekip, çalışmayı onaylamadan önce bir öneri, tasarım belgesi, proof of concept (PoC) veya daha küçük bir uygulama planı isteyebilir.

## Geliştirme Kuralları

Repository'nin sağladığı talimatları izleyin.

Bunlar şu konulardaki gereksinimleri içerebilir:

- Projeyi derleme ve çalıştırma
- Test
- Biçimlendirme ve lint
- Dokümantasyon
- Desteklenen platformlar
- Bağımlılık değişiklikleri
- Güvenlik açısından hassas işler
- Üretilen dosyalar
- Geriye dönük uyumluluk

Değişiklikleri odaklı tutun. Katkı için gerekli olmadıkça ilgisiz yeniden düzenlemelerden, biçimlendirme değişikliklerinden veya bağımlılık güncellemelerinden kaçının.

## Commit Mesajları

Octacity, Conventional Commits kullanır.

Aşağıdaki yapıyı kullanın:

```text
type(optional scope): description
```

Yaygın türler şunlardır:

```text
feat: add a new feature
fix: correct a bug
docs: update documentation
refactor: restructure code without changing behavior
test: add or update tests
build: change the build system or dependencies
ci: update continuous integration
chore: perform maintenance work
```

Örnekler:

```text
feat(auth): add session expiration
fix(parser): handle empty input safely
docs: clarify local setup instructions
refactor(storage): separate cache management
```

Değişikliği açıkça anlatan commit mesajları yazın. Repository'ler ek kurallar tanımlayabilir.

## Pull Request'ler

Pull request gereksinimleri, her repository'nin pull request şablonunda tanımlanır.

Genel olarak bir pull request:

- Onaylanmış veya tartışılmış bir issue'yu ele almalı
- Tek ve net bir amaca odaklanmalı
- Neyin neden değiştiğini açıklamalı
- İlgili issue'ya bağlantı vermeli
- Repository'nin teknik gereksinimlerine uymalı
- Uygun testleri veya doğrulamayı içermeli
- Davranış değiştiğinde dokümantasyonu güncellemeli
- Tamamlanmamış işleri veya bilinen sınırlamaları açıkça belirtmeli
- İnceleme geri bildirimine yapıcı biçimde yanıt vermeli

Bir pull request göndermek, birleştirileceğini garanti etmez.

İnceleyenler değişiklik isteyebilir, başka bir yaklaşım önerebilir, işi daha küçük katkılara bölebilir veya projeye uymadığında pull request'i reddedebilir.

## İnceleme ve Karar Alma

Her repository'nin, yönünden ve gelişiminin sürdürülmesinden sorumlu bir ekibi vardır.

Katkıların nasıl inceleneceğine ekip lideri karar verir. Ekip lideri:

- Katkıyı doğrudan inceleyebilir
- İncelemeyi ekibinden bir üyeye devredebilir
- Bir repository maintainer'ı atayabilir
- Başka bir Octacity ekibinin yetkin bir üyesinden inceleme isteyebilir

İnceleme yetkisi repository'den repository'ye değişebilir.

Bir katkının kabul edilmesi, gözden geçirilmesi, ertelenmesi veya reddedilmesi konusunda son karar sorumlu ekibe aittir.

İncelemeler şunlara odaklanmalıdır:

- Doğruluk
- Bakım yapılabilirlik
- Güvenlik
- Kapsam
- Projenin yönü
- Dokümantasyon
- Test
- Uyumluluk
- Uzun vadeli bakım maliyeti

## Yapay Zekâ Destekli Katkılar

Yapay zekâ destekli geliştirmeye izin verilir.

Octacity, katkıları bir yapay zekâ aracının kullanılıp kullanılmadığına göre değil; kalitelerine, dürüstlüklerine, bakım yapılabilirliklerine ve proje kurallarına uygunluklarına göre değerlendirir.

Gönderilen tüm işin sorumluluğu tamamen katkıyı gönderen kişiye aittir.

Bu, şunları yapmanız gerektiği anlamına gelir:

- Gönderdiğiniz kodu, metni, tasarımı veya diğer işi anlamak
- Yaklaşımı ve önemli kararları açıklayabilmek
- Katkının iddia edildiği gibi çalıştığını doğrulamak
- Üretilen çıktıyı hatalar, güvenlik sorunları ve uygunsuz değişiklikler açısından gözden geçirmek
- Repository'nin katkı ve lisans gereksinimlerine uymak
- İnceleme sırasında bizzat ve anlamlı biçimde yanıt vermek
- Gönderilen işte bulunan sorunları düzeltmek

Gözden geçirilmemiş, büyük miktarda üretilmiş içerik göndermeyin.

Katkıda bulunan kişi otomatik araçlar kullanıp sonucu anlamak veya doğrulamak için çaba göstermediğinde, inceleyenler tekrarlanan kural ihlallerine, özensiz çıktıya veya yanıltıcı iddialara karşı daha az hoşgörülü olabilir.

Octacity, otonom bir ajanla değil, katkıyı gönderen kişinin kendisiyle iletişim kurmayı bekler. Botlar ve ajanlar bağımsız olarak tartışma yürütmemeli, inceleyenlerle tartışmamalı veya kendilerini bir katkının sorumlu yazarı olarak sunmamalıdır.

## Saygılı İş Birliği

Tüm proje etkileşimlerinde Octacity [Davranış Kuralları](CODE_OF_CONDUCT_tr.md)'na uyun.

Teknik fikir ayrılığı hoş karşılanır; ancak tartışma yapıcı kalmalı ve işe odaklanmalıdır.

Şu konularda dürüst olun:

- Deneyiminiz
- Neyi anladığınız
- Neyi test ettiğiniz
- Nerede dış yardım aldığınız
- Bilinen sorunlar veya belirsizlikler
- İşin tamamlanıp tamamlanmadığı

Soru sormak teşvik edilir. Belirsizliği gizlemek edilmez.

## Güvenlik Sorunları

Repository açıkça böyle yapmanızı söylemediği sürece, şüphelenilen güvenlik açıklarını herkese açık bir issue üzerinden bildirmeyin.

Octacity [Güvenlik Politikası](SECURITY_tr.md)'nda veya repository'nin kendi güvenlik dokümantasyonunda anlatılan süreci izleyin.

## Lisans

Bir katkı göndererek, katkınızın repository'nin kullandığı lisans altında dağıtılabileceğini kabul etmiş olursunuz.

Katkıda bulunma hakkına sahip olmadığınız işleri göndermeyin.

Başka bir yerden kod, dokümantasyon, tasarım veya başka materyal uyarlarken kaynağı belirtin ve lisansının projeyle uyumlu olduğundan emin olun.

## Sorular

Açıklığa kavuşturulması gereken bir konu olduğunda repository'nin tanımladığı iletişim kanalını kullanın.

Projeye özel bir kanal yoksa, sorunuzu ve ilgili bağlamı anlatan bir issue açın.
