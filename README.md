## Özet​

Bu proje Türkiye, Rusya ve diğer ülkelerde bulunan engelli siteler ve uygulamalar için VPN'siz ve internet hızında yavaşlama olmadan girmek için GoodbyeDPI baz alınarak üzerine çeşitli düzenlemeler, hazır parametreler ve arayüz tasarlanmış bir versiyonudur. Ek özellikler barındırır. Gayet sade basit bir uygulamadır.

## Kaspersky Antivirüsü Kullananlar Hakkında Önemli Not
>
> [!CAUTION]
> Kaspersky isimli antivirüs yazılımı Rus hükümetiyle olan anlaşmasından dolayı bu uygulamada baz olarak kullanılan GoodbyeDPI'ın çalışmasına engel olmaktadır. Kaspersky isimli yazılımı kullanıyorsanız, kullandıysanız veya devre dışı halde bile olsa bilgisayarınızda bulunuyorsa lütfen tamamen kaldırın. Bunu yapmadığınız taktirde DPIUnlocker çok yüksek ihtimalle çalışmayacaktır. Kaspersky yerine alternatif antivirüs yazılımları tercih edebilir ya da Windows Defender kullanabilirsiniz. (Windows Defender 2025 yılı itibariyle kötü amaçlı yazılım ve siteleri engellemekte son derece yeterlidir.)
Kaspersky'i DPIUnlocker.exe dosyasının indirme işlemi sırasında devre dışı bırakmanız, indirdikten sonra dışlamalara eklemeniz veya devre dışı bırakmanız sorunu çözmeyecektir. DPIUnlocker'ı doğru şekilde kullanabilmek için Kaspersky isimli antivirüs yazılımından bir şekilde kurtulmalısınız.

## DPIUnlocker — Derin Paket İnceleme (DPI) Engellerini Atlatma Aracı

Bu uygulama, Türkiye'de Rusya'da ve diğer ülkelerde bazı internet servis sağlayıcılarının DNS değişikliğine izin vermemesi sebebiyle, bu durumu bertaraf etmek için asıl proje olan [GoodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI)'ın baz alınarak düzenlenmiş bir versiyonudur.
Bu yazılım, birçok ISS'da (İnternet Servis Sağlayıcısı) bulunan ve belirli web sitelerine erişimi engelleyen "Derin Paket İnceleme" (DPI) sistemlerini atlatmak için tasarlanmıştır.
Optik ayırıcı veya port yansıtma (Pasif DPI) kullanarak bağlanan ve herhangi bir veriyi engellemeyen, ancak istenen hedeften daha hızlı yanıt veren DPI'yi ve sıralı olarak bağlanan Aktif DPI'yi işler. Bu uygulama kesinlikle bir VPN değildir ve oyunlarda/genel internet kullanımında bir hız değişikliğine sebep olmayacaktır.

> [!NOTE]
> Windows 10 veya 11 64 Bit işletim sistemlerinde **yönetici olarak çalıştırmanız** mecburidir.

## DPIUnlocker ve Diğer Sansür Karşıtı Araçlar

- VPN'lerle karşılaştırma
	Etkinliği: DPIUnlocker ve VPN'ler sansürü etkili bir şekilde atlar, ancak DPIUnlocker özellikle DPI'ya karşı koymak için tasarlanmıştır.
	Hız: DPIUnlocker, trafiği VPN'ler gibi harici sunucular üzerinden yönlendirmediği için daha yüksek hızlar sunabilir.
	Gizlilik: VPN'ler tüm trafiği şifreleyerek daha iyi genel gizlilik sağlarken, DPIUnlocker DPI'yı atlamaya odaklanır.
- Proxy'lerle Karşılaştırma
	Etkinliği: Proxy'ler, DPIUnlocker ile karşılaştırıldığında DPI'ya karşı daha az etkilidir.
	Hız: DPIUnlocker, aracı sunuculara güvenmediği için genellikle daha iyi hız sunar.
	Gizlilik: Proxy'ler sınırlı gizlilik geliştirmeleri sunarken DPIUnlocker sansürü atlamaya odaklanır.

## Virüs & Veri Sızıntısı & Bitcoin Mining (ALINTI)

Program açık kaynak kodlu olduğundan tüm kodu görüp inceleyebilirsiniz. Bazı kullanıcılar VirusTotal'de false positive bildirimi yapsa da bu ``WinDivert.dll`` ve ``WinDivert64.sys`` dosyalarının fonksiyonlarından dolayı bu şekilde yanlış bir sonuç verebiliyor (bu dosyalar sistemi etkiler). Bu .dll ve .sys dosyaları da açık kaynak kodludur ve incelenebilir, yani tamamen temizdir. İstemeyen ve güvenmeyen kullanıcılar kullanmak zorunda değildir, herkesin kendi seçimidir.
Dilerseniz tüm klasörü ya da .zip dosyasını [VirusTotal](https://www.virustotal.com/gui/home/upload) gibi bir sitede taratıp sonuçları inceleyebilirsiniz.
> [!NOTE]
> **[VirusTotal sonuçlarında](https://www.virustotal.com/gui/file/3ca863444ce065361b1152e1dddae1147962fc78b90c17ff346efbb35bd146ee)** 73 adet antivirüs progamı içerisinde (bağlantıyla yönlendirileceğiniz sayfada 66 adet antivirüs programı bulunmakta çünkü bazıları ``.zip`` dosyalarını online taramayı desteklememekte) yalnızca Kaspersky isimli uygulama bu yazılımın zararlı olduğunu söylemektedir ancak bu hatalı bir uyarıdır (yukarıdaki uyarıyı okuyunuz). **Dolayısıyla Kaspersky kullanıyorsanız ya devre dışı bırakmanız ya da antivirüs programınızı değiştirmeniz önerilir.**

> [!IMPORTANT]
> WinDivert dosyalarının açıklamalarında ya da silmeye çalışırken karşılaşacağınız Bitcoin adresi sizi korkutmasın.
> WinDivert açık kaynaklı bir Windows Paket İnceleme-Değiştirme aracı kütüphanesidir. Bu kütüphanenin sahibi [basil00](https://github.com/basil00) isminde bir geliştiricidir. Bu geliştirici tamamen ücretsiz ve açık kaynak kodlu şekilde bu kütüphaneyi [Github - Windivert](https://github.com/basil00/WinDivert) isimli Github repository'sinde paylaşmaktadır.
> Bu geliştirici tamamen ücretsiz şekilde yayınladığı bu kütüphaneden hiçbir gelir elde etmemekte ancak kendisine gelecek bağışları da kabul etmektedir. Bağış yapılacak adres ise .dll ve .sys dosyalarının açıklamalarında bulunuyor. Yani gördüğünüz Bitcoin yazısı ve yanındaki karmaşık sayılar ve harflerden oluşan adres WinDivert kütüphanesinin geliştiricisi olan basil00'a ait bağış yapabileceğiniz **Bitcoin cüzdan adresidir.** Bu adresi resmi sitesinde de paylaşıyor, [bu da bağış sayfasının linki](https://reqrypt.org/donate.html).

## DPIUnlocker'ı Kullanmak

DPIUnlocker, sisteminizin bölgesel tercihlerine uygun ayarları otomatik yapar. Arayüzde ilgili sayfa karşınıza gelir ve kolayca kullanabilirsiniz. Türkiye, Rusya ve diğer ülkeler olmak üzere bölümlere ayrılmıştır. Genellikle uygulama açıldığında arayüzde varsayılan olarak en iyi konfigürasyon seçilmiştir. Tekrardan amacınıza hizmet etmek için yapılandırıp kaydedebilirsiniz. Türkiye için sistem başlangıçta çalıştırabilme seçeneği mevcuttur.

- DPI Modu: Derin Paket İncelemesini (DPI) aşmamıza olanak sağlayan değişken türü.
- DPI DNS: DPI seviyesinde DNS ayarı.
- DPI Engeli: Aşılmasını istediğiniz seçili olan engel haricinde diğer tüm internet trafiğine uygulanmaz. Sadece seçili engeli aşar ve diğer tüm trafikte oluşabilecek DPI tarafından oluşacak olumsuz durumları engellerisiniz.
- Sistem DNS: Sistem seviyesinde ağ adaptörlerine uygulanan DNS ayarı.
- Son Ayarı Koru(Keep Last Settings): ISP'niz için bulduğunuz veya kendinizin belirlediğiniz en iyi konfigürasyon ayarını daha sonra kullanabilmek için kaydeder.
- Sistem Açılınca Çalıştır (Sadece Türkiye): Belirlediğiniz ayarı bilgisayarınız açıldığı zaman otomatikmen başlatır ve sistem durumunda küçültür.
- Online Blacklist (Sadece Rusya): Rusya için sürekli güncellenen Rusyada engellenen sitelere ait listeyi kullanmaya yarar. [https://p.thenewone.lol/domains-export.txt]

> [!NOTE]
> İlk çalıştırmadaki açılış paketlenmiş uygulama olduğundan donanıma bağlı olarak ilk açılış biraz yavaş olabilir. Bir sonraki çalıştırmalarınızda böyle bir sorun olmayacaktır.
> DPIUnlocker'ın kullandığı tüm parametreler, sistem seviyesindeki ayarlar, kullanılmak için çıkarılan tüm geçici dosyalar uygulamayı normal koşullarrda kapattığınız sürece ayarlar temizlenir ve kullanım sonlandırılır.

## DPI DNS ve Port, Sistem DNS Ekleme, Düzenleme

Uygulmada bulunanan sizi karşılayan arayüzden DPI bazlı veya Sistem bazlı toplamda iki adet DNS seçebilirsiniz. 

- DPI DNS (Yandex DNS, Cloudflare, NextDNS) hazır olanlardan ISP'niz için en uygununu seçebilir veya --Kullanıcı-- seçeneğinden istediğiniz DNS adreslerini ve portunu girerek kullanabilirsiniz.
- Sistem DNS (Google, CloudFlare, NextDNS, Quad9, AdGuard, OpenDNS, Yandex, UncensoredDNS) hazır olanlardan seçip veya yine --Kullanıcı-- seçeneğinden isteğe göre girerek direkt sistem seviyesinde kullanabilirsiniz.

> [!NOTE]
> DPI DNS ilgili başlıktan herhangi bir DNS parametresi seçili iken sistem seviyesinde DNS kullanılamaz çünkü DPI konfigürasyonu olarak seçildiğinde sistem seviyesindeki DNS pasif kalır. DPI DNS > Sistem DNS
> Sistem seviyesinde DNS seçildiğinde sistemdeki mevcut tüm ağ adaptörlerine uygulanır. Uygulamayı normal koşullarda kapatığınız sürece ağ adaptörlerinde bulunan DNS ayarları sıfırlanır.

## DPIUnlocker Nasıl Çalışır?

GoodbyeDPI, veri paketlerinin ağ üzerinden gönderilme şeklini değiştirerek onları DPI sistemleri tarafından daha az tanınabilir hale getirir. GoodbyeDPI tarafından kullanılan birincil yöntemler şunları içerir:

- Paketleri parçalama: Veri paketlerini, DPI sistemlerinin analiz etmesi daha zor olan daha küçük parçalara bölmek.
- Paket imzalarını değiştirme: Paket başlıklarını daha az algılanabilir hale getirmek için değiştirme.
- Sahte paket uzunlukları kullanma: DPI sistemlerini karıştırmak için paket uzunluklarını değiştirmek.

Bu teknikler, DPI sistemlerinin amaçlanan trafiği doğru bir şekilde tanımlamasını ve engellemesini zorlaştırarak kullanıcıların sansürü atlamasına ve kısıtlı içeriğe erişmesine olanak tanır.

## Sık Karşılaşılan Sorunlar

- DPIUnlocker başlatılamdıysa veya görev yöneticisi işlemler menüsünde GoodbyeDPI görünmüyorsa (Yalancı virüs algılaması):
Uygulamayı veya bulunduğu konumu antivirüs programınıza dışlama/istisna olarak ekleyin. Windows Defender kullanıyorsanız [buradaki rehberi](https://support.microsoft.com/tr-tr/windows/windows-g%C3%BCvenli%C4%9Fi-ne-d%C4%B1%C5%9Flama-ekleme-811816c0-4dfd-af4a-47e4-c301afe13b26) (Kaspersky antivirüs programında hiç bir şekilde dışlama/istisna kabul edilmiyor programdan kurtulmalısınız. Uyarıyı Okuyunuz.)

- Bazı sitelerin yavaş açılması/açılmaması sorunu:
Bu sorunu komut dosyalarında TTL ayarı bulunan yöntemlerde yaşayabilirsiniz. Eğer belirli siteler yavaş açılıyor ya da hiç açılmıyorsa TTL ayarı içermeyen DPI Modunu seçebilirsiniz.

- Discord'a web üzerinden giriş yapabilmeye rağmen uygulamanın açılmaması sorunu: (ALINTI)
Bu sorun genellikle fiber tarife kullanıcılarının karşılaştığı bir sorun ve maalesef kesin bir çözüm yolu yok. Ancak yine de bu çözüm yolunu deneyebilirsiniz: **[WinDivertTool.exe](https://github.com/basil00/WinDivertTool/releases/download/v2.2.0/WinDivertTool.exe)** isimli WinDivert tanı aracını indirip çalıştırdıktan sonra konsol penceresinin en altında yer alan listede hangi uygulamaların WinDivert kullanarak çalıştığını görebilirsiniz. Bu listede birden fazla uygulama var ise ilgili satırlarda bulunan konuma giderek söz konusu uygulamayı veya uygulamaları siliniz. Yalnızca en son kurduğunuz konumdaki WinDivert kütüphanesini kullanan uygulamayı silmeyiniz. Ardından bilgisayarınızı yeniden başlatarak doğru şekilde çalışıp çalışmadığını deneyebilirsiniz. 

- Ethernet bağlantısı sorunu: (ALINTI)
İnternet bağlantınızı ethernet adaptörü aracılığı ile sağlıyorsanız ve GoodbyeDPI tüm çözümleri denemenize rağmen GoodbyeDPI'ı çalıştaramadıysanız **harmanprecious** isimli kullanıcıya ait çözüm rehberine **[bu adresten](https://www.technopat.net/sosyal/konu/goodbyedpi-ethernet-kartiyla-calismiyorsa-ne-yapilmali.3619948/)** adresinden ulaşabilirsiniz.

## Yasal Uyarı
>
> [!IMPORTANT]
> Bu uygulamanın kullanımından doğan her türlü yasal sorumluluk kullanan kişiye aittir. Uygulama yalnızca eğitim ve araştırma amaçları ile yazılmış ve düzenlenmiş olup; bu uygulamayı bu şartlar altında kullanmak ya da kullanamamak kullanıcının kendi seçimidir. Açık kaynak kodlarının paylaşıldığı bu platformdaki düzenlenmiş bu proje, bilgi paylaşımı ve kodlama eğitimi amaçları ile yazılmış ve düzenlenmiştir.
