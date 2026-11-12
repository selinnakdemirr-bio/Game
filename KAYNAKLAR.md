# Doz Sıfır — Fikirden Rafa · Kaynaklar, basitleştirmeler, test listesi

> Eğitim amaçlı kurgudur, tıbbi tavsiye değildir. Oyunu açmak için `index.html` dosyasını bir tarayıcıda açın (çevrimdışı çalışır).
> Geliştirici kısayolu: `index.html?ch=5` 5. duraktan başlatır; `?debug` test için `window.__doz` nesnesini açar.

## 1) Mit–kanıt tablosu

| # | Durak | Mit | Kanıt (oyundaki doğru seçenek) | Kaynak |
|---|---|---|---|---|
| 1 | Sinyal | mRNA aşısı DNA’mı değiştirir | mRNA çekirdeğe girmez, DNA’ya ulaşmaz, hücrede parçalanır; viral vektör de genoma entegre olmaz | [CDC Mitler ve Gerçekler (arşiv)](https://archive.cdc.gov/www_cdc_gov/covid/vaccines/myths-facts.html) · [AMA](https://www.ama-assn.org/system/files/covid-vaccine-myths-facts.pdf) |
| 2 | Laboratuvar | Aşı fetal doku içerir | Bazı aşıların üretiminde/testinde uzun süredir kullanılan hücre hatları (HEK293, PER.C6) yer aldı; arındırılmış nihai üründe fetal doku/hücre yok | [CHOP – Fetal hücreler](https://www.chop.edu/vaccine-education-center/vaccine-safety/vaccine-ingredients/fetal-tissues) · [Science Feedback](https://science.feedback.org/review/although-fetal-cell-lines-are-used-to-grow-viruses-for-some-covid-19-vaccines-the-cells-are-not-part-of-the-vaccines/) |
| 3 | Preklinik | Aşı beni hasta eder | Canlı virüs içermez; ateş, yorgunluk, kol ağrısı bağışıklık yanıtının işaretidir ve genellikle birkaç günde geçer | [CDC (arşiv)](https://archive.cdc.gov/www_cdc_gov/covid/vaccines/myths-facts.html) · [CT Aşı Portalı](https://portal.ct.gov/vaccine-portal/vaccine-knowledge-base/articles/will-the-vaccine-give-me-covid-19) |
| 4 | Klinik fazlar | Çok hızlı yapıldı, güvenli olamaz | Genom hızla paylaşıldı; önceki koronavirüs ve mRNA araştırmaları; fazlar üst üste bindi; kademeli inceleme; risk altında erken üretim; on binlerce katılımcı | [Gavi VaccinesWork](https://www.gavi.org/vaccineswork/how-did-scientists-manage-develop-safe-covid-19-vaccines-just-ten-months) · [APhA](https://vaccineconfident.pharmacist.com/Learn/Vaccine-Confident-Playbook/Addressing-concerns-that-the-COVID-19-vaccines-were-rushed) |
| 5 | Düzenleyici | Aşı kısırlık yapar | Kanıt yok. Büyük bir mRNA aşısının Faz III denemesinde istenmeden oluşan gebelikler gruplar arasında benzerdi (12 aşı / 11 plasebo); sayı küçük, asıl güvence sonraki gözlemsel veriler | [Mayo Clinic Health System](https://www.mayoclinichealthsystem.org/hometown-health/featured-topic/covid-19-vaccine-myths-debunked) · [Nebraska Medicine](https://nebraskamed.com/node/20596) · [Quartz – “sayfa 132”](https://qz.com/1950810/what-to-know-about-page-132-of-the-pfizer-vaccine-report/) |
| 6 | Üretim | Aşıda mikroçip var | Yok. İçerik: mRNA, lipitler, tuzlar, şekerler, asitlik düzenleyiciler | [CDC (arşiv)](https://archive.cdc.gov/www_cdc_gov/covid/vaccines/myths-facts.html) |
| 7 | Soğuk zincir | Hastalığı geçirdim, aşı gereksiz *(tarihe duyarlı)* | Enfeksiyon sonrası bağışıklığın düzeyi ve süresi kişiden kişiye değişir; bir çalışmada önceden enfekte yetişkinlerde mRNA aşısı hastaneye yatışa karşı ek koruma sağladı. Oyun öneri vermez, hekime/sağlık otoritesine yönlendirir | [CDC MMWR 2022;71(15)](https://www.cdc.gov/mmwr/volumes/71/wr/mm7115e2.htm) · [CT Aşı Portalı](https://portal.ct.gov/vaccine-portal/vaccine-knowledge-base/articles/vaccination-after-getting-covid) |
| 8 | Halkla buluşma | Riskleri gizlediler | Miyokardit sinyali aşı sonrası izlemeyle yakalandı, açıklandı, ürün bilgisine eklendi; nadir, çoğunlukla genç erkeklerde, 2. dozdan sonraki günlerde. ABD 2021: 12–29 yaş erkeklerde 2. dozdan sonra ~40,6 bildirim/milyon doz. 12–17 yaş erkeklerde enfeksiyon sonrası kalp komplikasyonu riski 2. doz sonrasının 1,8–5,6 katı | [CDC MMWR 2021;70(27)](https://www.cdc.gov/mmwr/volumes/70/wr/mm7027e2.htm) · [CDC MMWR 2022;71(14)](https://www.cdc.gov/mmwr/volumes/71/wr/mm7114e1.htm) |
| 9 | İzleme | Bildirilen her olay aşıdan kaynaklanır | Pasif bildirim erken uyarı aracıdır; tek başına rapor nedensellik göstermez; neden belirsiz olsa bile bildirim istenir | [VAERS SSS](https://vaers.hhs.gov/faq.html) · [CDC WONDER – VAERS](https://wonder.cdc.gov/vaers.html) |

Not: CDC’nin canlı mit sayfası taşındığı için arşiv kopyası kullanıldı. Kaynaklar 2021–2024 tarihlidir; önerilerle ilgili güncel bilgi için ulusal sağlık otoritesine bakılmalıdır.

## 2) Bilimsel basitleştirmeler

- **Genom haritası** yaklaşık oranlarla çizildi (ORF1ab, S, ORF3a, E, M, ORF6–8, N); harf dizisi rastgele üretilir.
- **Antijen tasarımı** “füzyon öncesi şekli sabitle” seçimine indirgendi; prolin ikamesi gibi ayrıntılar anlatılmadı.
- **Laboratuvar akışı** kurgusal bir test protokolüdür: Gerçek mRNA-LNP formülasyonu mikroakışkan karıştırma ile yapılır, pipetle değil. “Sükrozlu stok” viskoz sıvı örneği olarak seçildi.
- **Pipet fiziği**: Damlama/aerosol eşikleri, 4 px = 1 mm ölçeği, eğim (harekete bağlı sarkaç) oyun tasarımı değerleridir; gerçek hacim hataları ölçülmez.
- **Resüspansiyon** yatay sallama olarak modellendi; gerçekte çoğunlukla pipetle yukarı-aşağı karıştırılır. Liziz/denatürasyon tek bir “sertlik” eşiğine bağlandı.
- **ELISA**: Tek plaka, 3 satır, 8 seyreltme; eşik = “boş kuyucuğun 2 katı” (yaygın ama tek kural değil). OD değerleri ve 1:6400 titresi kurgusaldır.
- **Klinik deneme**: 8+8 gönüllü görseli; 10.000/10.000 kişilik vaka sayıları (80 vs 8, %90) kurgusaldır. Zaman çizelgesi ölçeksizdir; faz süreleri sabit tutuldu (gerçekte yaygın bulaş Faz III’te vaka birikimini de hızlandırdı).
- **Düzenleyici süreç** genel adlarla anlatıldı; ülkeye özgü kurum ve prosedür adı kullanılmadı.
- **Kalite kontrol** dört parametreye (sterilite, mRNA bütünlüğü, LNP partikül boyutu, saflık) ve geçti/kaldı sonucuna indirgendi.
- **Soğuk zincir** sıcaklığı birimsiz bir ölçekle ve “etiketteki üst sınır” olarak gösterildi; ürünlere özgü derece aralıkları yazılmadı.
- **İzleme**: Gözlenen/beklenen grafiği ve aktif takip animasyonu kurgusaldır; gerçek sinyal analizleri istatistiksel yöntemler içerir.
- **Final kapsam yüzdesi** güven, stabilite, kontaminasyon ve hata sayısından türetilen bir oyun skorudur.

## 3) Test kontrol listesi

- [x] Konsolda hata/uyarı yok (Playwright, 9 durak + final uçtan uca)
- [x] Masaüstü 1366×820, telefon dikey (iPhone 13) ve yatay 844×390 düzenleri
- [x] Dokunmatik: dokunma ile başlatma, diyalog atlama, sahne etkileşimi
- [x] Açılışta “Eğitim amaçlı kurgudur, tıbbi tavsiye değildir.” ve siyah-beyaz Doz Sıfır logosu
- [x] Durum makinesi: INTRO → CHAPTER_n → PHASE_DONE → … → WIN; FAIL → “yeniden dene” (metrikler durak başına geri yüklenir)
- [x] FAIL tetikleyicileri: kontaminasyon ≥75, canlılık <40, stabilite <15, güven <12, 2 hatalı parti, soğuk zincir sapması
- [x] Lab: eldiven → ısı dengesi → dengeli santrifüj (yanlış yuvada sarsılma) → resüspansiyon (sert = liziz geri bildirimi) → ileri teknik → uç atma → yeni uç → ters teknik → hücrelere ekleme
- [x] Pipet: piston 1./2. kademe dikey sürükleme ve kademe direnci; hızlı bırakma = kabarcık; derinlik/açı kesit paneli; hızlı taşıma = damla/aerosol; kullanılmış uçla yeni reaktif = çapraz kontaminasyon
- [x] Hız çubuğu yok; geri bildirim nesne üzerinde (dalga, damla, köpük, renk, sarsılma)
- [x] Her an tek adım parlar (spot ışığı), diğerleri soluklaşır; “Ne yap?/Neden?” kartı ve hata açıklaması
- [x] 9 Mit Avı kartı: Mit → Neden inanılıyor → Kanıt → Doğru açıklama → Kaynak etiketi; koleksiyon ekranı
- [x] 8. durak: Halk Güveni göstergesi; alay/baskı/abartı güveni düşürür; kanıt kartı sunma
- [x] Final: halk güveni, kapsam, “Gerçek hayatta güvenilir kaynak nerede?” ekranı ve hekime yönlendirme
- [ ] Gerçek cihazlarda (iOS Safari, Android Chrome) elle oynanış ve ekran okuyucu denetimi önerilir
