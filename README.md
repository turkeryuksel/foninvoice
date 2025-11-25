# Fon Cosmetics - Pro Panel (Fatura Sistemi)

Bu proje, Firebase tabanlı, tek sayfalık bir fatura yönetim sistemidir.

## 🚀 Kurulum ve Çalıştırma

Bu proje statik bir web sitesidir (`index.html`). Ancak Firebase Authentication ve diğer modern web özelliklerinin düzgün çalışması için **yerel bir sunucu** üzerinden çalıştırılmalıdır. Dosyaya çift tıklayarak (`file://`) açmak bazı özelliklerin çalışmamasına neden olabilir.

### 1. Yerel Olarak Çalıştırma (Tavsiye Edilen)

Eğer bilgisayarınızda Python yüklü ise:

1.  Terminali açın ve proje klasörüne gidin.
2.  Aşağıdaki komutu çalıştırın:
    ```bash
    python3 -m http.server 8000
    ```
3.  Tarayıcınızda `http://localhost:8000` adresine gidin.

Veya VS Code kullanıyorsanız "Live Server" eklentisi ile `index.html` dosyasını açabilirsiniz.

### 2. GitHub Pages'de Yayınlama

Bu projeyi GitHub Pages üzerinden yayınlayabilirsiniz.

1.  Bu repoyu GitHub'a yükleyin.
2.  Repo ayarlarından (Settings) -> **Pages** bölümüne gidin.
3.  **Source** olarak `main` (veya `master`) dalını seçin ve kaydedin.
4.  GitHub size sitenizin yayınlandığı linki verecektir (örn: `https://kullaniciadi.github.io/repo-adi/`).

## ⚠️ ÖNEMLİ: Firebase Ayarları

Projenin giriş yapabilmesi ve çalışabilmesi için Firebase Console üzerinden alan adınıza izin vermeniz gerekir.

1.  [Firebase Console](https://console.firebase.google.com/)'a gidin.
2.  **Authentication** menüsüne tıklayın.
3.  **Settings** (Ayarlar) sekmesine gidin.
4.  **Authorized Domains** (Yetkili Alan Adları) kısmına gelin.
5.  **Add Domain** diyerek GitHub Pages alan adınızı ekleyin (örn: `turkeryuksel.github.io`).

Bunu yapmazsanız giriş yaparken hata alırsınız.

## Özellikler

-   **Fatura Oluşturma**: Proforma ve Commercial faturalar.
-   **PDF Çıktısı**: A4 formatında, düzgün sayfa yapısı ile PDF indirme.
-   **Excel Çıktısı**: Faturayı Excel formatında indirme.
-   **Otomatik Kayıt**: Müşteri ve ürün bilgileri otomatik hatırlanır.
-   **Çoklu Para Birimi**: USD, EUR, TL, RUB desteği.
