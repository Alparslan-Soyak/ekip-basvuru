# 🚀 DEÜ Etkinlikleri - Ekip Başvuru Altyapısı

Bu depo (repository), **DEÜ Etkinlikleri** topluluğunun yeni dönem ekip alımları için tasarlanmış yönlendirme ve arayüz altyapısını barındırmaktadır. Ana web sitesinin bütünlüğünü bozmamak adına tamamen bağımsız bir alt alan adı (subdomain) üzerinde çalışacak şekilde mimari edilmiştir.

---

## 🌐 Canlı Yayın Bilgileri
* **Nihai Link:** `https://basvuru.deuetkinlikleri.com` ve `https://ekip-basvuru.vercel.app/`
* **Barındırma Altyapısı (Hosting):** Vercel (Production Environment)
* **Alan Adı Sağlayıcısı (Domain):** Namecheap

---

## 🛠️ Teknik DNS Yapılandırması (Namecheap Ayarları)

Mevcut ana sitenin (`deuetkinlikleri.com`) "Tadilat" sayfasına zarar vermemek için bu proje **CNAME Yönlendirmesi** ile bağlanmıştır. Namecheap panelindeki *Advanced DNS* sekmesinde yer alan aktif kayıt şu şekildedir:

| Tür (Type) | Ana Bilgisayar (Host) | Değer (Value) |
| :--- | :--- | :--- |
| `CNAME Record` | `basvuru` | `0aff0f7015306bfd.vercel-dns-017.com.` |

---

## 📂 Proje Dosya Yapısı ve Güncelleme Rehberi

* **`index.html`**: Sitenin ana iskeletidir. Logolu header, buzlu cam (glassmorphism) efektli konteyner ve buton tasarımları bu dosyadadır.
* **`logo-1.png`**: Sol üstte topluluk adının yanında konumlanan resmi DEÜ Etkinlikleri logosudur.

### 🔗 Google Form Linklerini Değiştirme:
Gelecek dönemlerde başvuru formlarının linkleri değiştiğinde veya yeni formlar açıldığında:
1. `index.html` dosyasını düzenleme moduna alın.
2. Dosyanın en altında yer alan `href="LINK_BURAYA_..."` alanlarındaki eski linkleri silip yeni Google Form linklerinizi yapıştırın.
3. Değişiklikleri `Commit changes` diyerek kaydedin. Vercel yeni linkleri saniyeler içinde canlıya alacaktır.

---

## ⚖️ Lisans ve Haklar
© 2026 DEÜ Etkinlikleri - Tüm Hakları Saklıdır.
