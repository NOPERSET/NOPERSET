# 04 Programı

Bu proje, verilen dört sayıyı kullanarak sıfır sonucuna ulaşmayı hedefleyen bir interaktif matematik oyunudur. Kullanıcı dört sayıyı girer ve bu sayılarla toplama, çıkarma, çarpma veya bölme işlemleri yaparak sıfır sonucuna ulaşmaya çalışır. Oyun, görsel ve ses efektleriyle zenginleştirilmiştir.

## Özellikler
- **Oyun Modu:** Kullanıcı, dört sayıyı (örneğin 6, 3, 2, 1) kullanarak sıfır sonucuna ulaşmaya çalışır.
- **Zorluk Seviyeleri:** Kolay (600 saniye), Orta (300 saniye) ve Zor (150 saniye) modları mevcuttur.
- **Çözüm Bulucu:** Kullanıcı dört sayıyı girip "Çöz" butonuna bastığında, oyun otomatik bir çözüm üretir.
- **İpucu Desteği:** Oyun sırasında "İpucu" butonuna basarak yardım alabilirsiniz (maksimum 3 ipucu).
- **Kalan Sayılar Bilgisi:** Her adımda kalan sayılar bilgi kutusunda gösterilir.
- **Medya Desteği:** Arka plan resmi, logo, arka plan müziği ve kazanma sesi ile oyun daha eğlenceli hale getirilmiştir.

## Kurulum ve Çalıştırma
Bu proje, tek bir HTML dosyası (`index.html`) ve medya dosyalarını içeren bir `assets` klasörü ile çalışır. Herhangi bir ek bağımlılık gerektirmez.

### Yerel Olarak Çalıştırma
1. Proje dosyalarını indirin veya kopyalayın.
2. `04-Programi` klasörünü bir web tarayıcısında (Chrome, Firefox vb.) açmak için `index.html` dosyasını çift tıklayın.
3. Dört sayıyı girerek oyunu oynayabilir, "Çöz" butonuna basarak otomatik çözümü görebilirsiniz. Arka plan müziği ve resimlerin çalıştığını kontrol edin.

### Netlify Üzerinde Yayınlama
1. Netlify hesabınıza giriş yapın.
2. Yeni bir site oluşturun veya mevcut bir siteyi kullanın (örneğin `spontaneous-pony-4dcccc`).
3. Aşağıdaki dosya yapısını hazırlayın:04-Programi/ ├── index.html ├── _redirects ├── README.md ├── assets/ ├── images/ │   ├── background.jpg │   ├── logo.png ├── sounds/ │   ├── background-music.mp3 │   ├── win-sound.mp3- `_redirects` dosyasının içeriği:
  ```
  /* /index.html 200
  ```
4. Netlify panelinde **"Deploys"** sekmesine gidin.
5. "Drag and drop your site output folder here" kısmına `04-Programi` klasörünü sürükleyip bırakın.
6. Yükleme tamamlandıktan sonra "Clear cache and deploy site" seçeneğini kullanarak önbelleği temizleyin.
7. Site URL’nizi (örneğin `https://spontaneous-pony-4dcccc.netlify.app/`) tarayıcıda açın ve oyunu test edin.

### GitHub ile Kullanım (Opsiyonel)
1. GitHub hesabınıza giriş yapın ve `04-Programi` adında bir repository oluşturun.
2. Tüm dosyaları (including `assets` klasörünü) GitHub’a yükleyin.
3. Netlify’yi GitHub reposuna bağlayın:
- Netlify panelinde "Link repository" seçeneğiyle GitHub hesabınızı bağlayın.
- `04-Programi` reposunu seçin ve "Deploy site" butonuna basın.
4. Değişiklikler yaptıkça GitHub’a commit edip push yaparak siteyi otomatik güncelleyebilirsiniz.

## Kullanım
- **Oyun Oynama:**
1. Dört sayıyı (örneğin 6, 3, 2, 1) girin.
2. "Oyna" butonuna basın ve bir zorluk seviyesi seçin (Kolay, Orta, Zor).
3. Her adımda iki sayıyı seçin, bir işlem (+, -, *, /) yapın ve sonucu girin.
4. Tüm sayıları kullanarak sıfır sonucuna ulaşmaya çalışın. Oyunu kazandığınızda bir kazanma sesi çalar.
- **Çözüm Bulma:**
1. Dört sayıyı girin.
2. "Çöz" butonuna basın, otomatik çözüm adımları ekranda görünecek.
- **Medya Özellikleri:**
- Arka plan müziği, oyun başladığında otomatik çalar.
- Oyunu kazandığınızda `win-sound.mp3` çalar.
- Arka plan resmi (`background.jpg`) ve logo (`logo.png`) görsel olarak siteyi süsler.

## Örnek
Sayilar: 6, 3, 2, 1  
Hedef: 0  
Çözüm adımları:
- 3 + 2 = 5
- 5 + 1 = 6
- 6 - 6 = 0

## Geliştirici Notları
- Proje tamamen HTML, CSS ve JavaScript kullanılarak yazılmıştır.
- Medya dosyaları `assets` klasöründe saklanır:
- `images/` için: `background.jpg` ve `logo.png`.
- `sounds/` için: `background-music.mp3` ve `win-sound.mp3`.
- Herhangi bir harici kütüphane veya bağımlılık yoktur.
- Netlify’de çalıştırırken `_redirects` dosyasını eklemek önemlidir, çünkü bu bir Single-Page Application (SPA) yapısındadır.
- Dosya yolları (`assets/images/background.jpg` gibi) doğru olmalıdır, aksi halde medya dosyaları yüklenmez.

## Yazar
- **NOPERSET**

## Lisans
Bu proje kişisel kullanım için yazılmıştır. Ticari kullanım için lütfen iletişime geçin.
