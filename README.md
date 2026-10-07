<p align="center">
  <img src="icons/logo.svg" alt="HORRORMAX" width="400">
</p>

<h3 align="center">Sadece korku filmlerinden oluşan, Netflix tarzı bir film kütüphanesi</h3>

<p align="center">
  <a href="https://fahriefe.github.io/horrormax/"><b>▶ Canlı demo</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/fahriefe/horrormax_app">Uygulama sürümü</a>
</p>

<p align="center">
  <img alt="HTML" src="https://img.shields.io/badge/HTML5-e34f26?style=flat-square&logo=html5&logoColor=white">
  <img alt="CSS" src="https://img.shields.io/badge/CSS3-1572b6?style=flat-square&logo=css3&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-f7df1e?style=flat-square&logo=javascript&logoColor=black">
  <img alt="SVG" src="https://img.shields.io/badge/SVG-ffb13b?style=flat-square&logo=svg&logoColor=black">
  <img alt="Responsive" src="https://img.shields.io/badge/responsive-mobil%20uyumlu-e50914?style=flat-square">
</p>

<p align="center">
  <img src="screenshots/01-anasayfa.jpg" alt="Ana sayfa" width="820">
</p>

---

## 🎬 Proje hakkında

**HORRORMAX**, 478 korku filmini 16 alt türe ayıran, Netflix benzeri bir film kütüphanesidir. Ana sayfada filmin afişi ve sahnesiyle öne çıkan büyük bir alan, her alt tür için yatay kaydırmalı satırlar, arama ve film detayları bulunur.

Bir **oyunlaştırma katmanı** da var: izlediğin filmleri işaretlersin, bir serinin tüm filmlerini bitirince o seriye özel çizilmiş bir **rozet** kazanırsın, rozetlerini profilinde sergilersin.

> Bu depo, projenin **web sitesi / portfolyo** sürümüdür: sunucu ya da hesap gerektirmez, herkes gezebilir. Kullanıcı hesaplı, telefona kurulabilen **uygulama sürümü** [ayrı bir depoda](https://github.com/fahriefe/horrormax_app) tutulur ve **şahsi kullanım** içindir.

## ✨ Öne çıkanlar

- 🎞 **478 film, 16 alt tür:** Slasher, Hayalet, Şeytani, Zombi, Vampir, Psikolojik, Found Footage, Body Horror, Folk Horror, Gore, Korku-Komedi, Yaratık, Asya, Kozmik, Hayatta Kalma, Gotik
- 📚 **88 film serisi koleksiyonu:** Halloween, Elm Street, Scream, Saw gibi serilerin tüm filmleri ve devam filmleri bir arada
- 🏅 **88 özel çizim rozet:** her seri için elle tasarlanmış SVG rozetler (ör. Texas Chain Saw için Leatherface'in kanlı testeresi)
- 👁 **İzlediklerim:** izlediğin filmler renkli, izlemediklerin gri; izlenenler öneri listelerinden çıkar
- 👤 **Profil:** profil resmi, lakap, rozet vitrini
- 🔎 Arama, alt tür filtreleri, "serinin diğer filmleri" ve "benzer filmler"
- 📱 **Mobil uyumlu:** telefonda alt sekme çubuğu, parmakla kaydırma, dokunmatik dostu kartlar
- 🎨 Akıcı animasyonlar: kart çıkışları, rozet kazanma ekranı, sayfa konumunu bozmayan yeniden çizim

<p align="center">
  <img src="screenshots/02-koleksiyonlar.jpg" alt="Koleksiyonlar" width="400">
  <img src="screenshots/03-profil-rozetler.jpg" alt="Profil ve rozetler" width="400">
</p>
<p align="center">
  <img src="screenshots/04-film-detay.jpg" alt="Film detayı" width="400">
  <img src="screenshots/05-mobil.jpg" alt="Mobil görünüm" width="190">
</p>

## 🛠 Teknik notlar

- **Çatısız (vanilla) tek sayfa uygulama:** HTML, CSS ve JavaScript; derleme adımı ya da bağımlılık yok. Statik barındırmada (GitHub Pages) çalışır.
- **Veri modeli:** filmler alt türlere göre gruplanmış bir dizide; seriler (koleksiyonlar) film adı kalıplarıyla otomatik oluşturulur.
- **Rozetler:** her koleksiyon için SVG çizimler, küçük yardımcı fonksiyonlarla (`P`, `C`, `E`, `R`, `L` gibi) kodla üretilir; altıgen çerçeve ve parlama animasyonu CSS ile yapılır.
- **Kalıcılık:** izlediklerin, listen, rozetlerin, lakabın ve profil resmin ziyaretçinin tarayıcısında (`localStorage`) saklanır; sunucuya kişisel veri gitmez. Profil resmi tarayıcıda kırpılıp küçültülür.
- **Akıcı arayüz:** FLIP tekniğiyle kart kaybolma animasyonları, kaydırma konumunu koruyan "yumuşak yeniden çizim", sabit sıralı rastgele öneriler.
- **Mobil:** `viewport-fit`, güvenli alan (safe-area) boşlukları, dokunmatik cihazlarda her zaman görünen düğmeler.
- **Görseller:** afişler ve sahneler [TMDB](https://www.themoviedb.org/) üzerinden gösterilir, depoda saklanmaz.

## 🚀 Yerelde çalıştırma

Kurulum gerekmez. Depoyu indir ve herhangi bir statik sunucuyla aç:

```bash
python -m http.server 8000
# sonra http://localhost:8000 adresini aç
```

## 📂 Yapı

```
index.html     uygulamanın tamamı (arayüz + mantık)
veri/          filmler, Türkçe açıklamalar, rozet verileri ve çizimleri
icons/         logo ve favicon
screenshots/   ekran görüntüleri
```

## 🖼 Atıf ve not

Film bilgileri ve Türkçe açıklamalar bu proje için hazırlanmıştır; IMDb puanları yaklaşık değerlerdir. Bu proje kâr amacı gütmez, bir portfolyo çalışmasıdır.

<sub>Bu ürün TMDB API'sini kullanır ancak TMDB tarafından onaylanmamış veya sertifikalandırılmamıştır.</sub>
