# SAP Business One Belge İptal Aracı — Vitrin ve Dokümantasyon 📄⚙️

[English](README.md) | **Türkçe**

**SAP Business One üzerinde 23 farklı belge türünü toplu olarak listeleme, ön kontrollerden geçirme, ters kayıtla iptal etme ve desteklenen belgeleri kapatma masaüstü uygulaması.**

> ℹ️ **Bu Vitrin Hakkında:**  
> Bu depo **ürün tanıtımı ve teknik portföy** içindir. Uygulama kaynak kodları (C#, .NET, SAP Service Layer ve DI API entegrasyon katmanı) şirket içi **private** depoda tutulmaktadır. Burada uygulamanın yetenekleri, desteklenen belge türleri ve örnek verilerle alınmış ekran görüntüleri yayımlanmaktadır.

---

## 📸 Ekran Görüntüleri ve Arayüz Galerisi

| Ana Ekran (Toplu Belge Listeleme ve İptal Paneli) |
|---|
| ![Ana Ekran](images/tr/overview.png) |

| Belge Türleri Seçimi (23 Farklı SAP Belgesi) | Belge Detayları ve Satır Kalemleri |
|---|---|
| ![23 Belge Türü](images/tr/document-types.png) | ![Belge Detayı](images/tr/document-details.png) |

| İşlem Öncesi Kontrol ve Onay Penceresi | Ayarlar ve SAP Bağlantı Yönetimi |
|---|---|
| ![Ön Kontrol](images/tr/precheck.png) | ![Ayarlar](images/tr/settings.png) |

| Kullanıcı Girişi | Yardım ve Kılavuz |
|---|---|
| ![Giriş](images/tr/login.png) | ![Yardım](images/tr/help.png) |

---

## 🎯 Temel Yetenekler ve Mühendislik Detayları

* **23 Farklı Belge Türü Desteği:** Satış, Satınalma, Stok ve Finans modüllerindeki tüm temel SAP Business One belgelerini kapsar.
* **İşlem Öncesi Güvenlik Kontrolleri (Pre-Checks):** Belgenin daha önce iptal edilip edilmediği, döneminin kapalı olup olmadığı veya ilişkili ardıl belgelerinin (örneğin faturaya dönüşmüş irsaliye) bulunup bulunmadığı işlem öncesinde denetlenir; hatalı işlemler engellenir.
* **Toplu Veri Yükleme (Batch Processing):** Belge numaraları Excel dosyalarından (`.xlsx`, `.xls`), metin dosyalarından veya doğrudan panodan (clipboard) yapıştırılarak tek seferde yüzlerce satır halinde içeri aktarılabilir.
* **Çift Dilli Arayüz (EN & TR):** Türkçe ve İngilizce dil desteği, yerel tarih ve para birimi formatları.
* **Denetim ve Loglama:** Gerçekleşen tüm iptal ve kapatma işlemleri zaman damgası, kullanıcı adı, SAP hata/başarı mesajları ve işlem loglarıyla birlikte Excel formatında dışa aktarılabilir.

---

## 📋 Desteklenen SAP Business One Belge Türleri

| Modül | Desteklenen Belgeler |
|---|---|
| **Satış (A/R)** | Müşteri Faturası (A/R Invoice), Alacak Dekontu (Credit Memo), Peşinat Faturası (Down Payment), Teslimat/İrsaliye (Delivery), Müşteri İadesi (Returns), Satış Siparişi (Sales Order), Satış Teklifi (Quotation) |
| **Satınalma (A/P)** | Satıcı Faturası (A/P Invoice), Satıcı Alacak Dekontu, Satıcı Peşinatı, Mal Girişi İrsaliyesi (GRPO), Mal İadesi, Satınalma Siparişi (Purchase Order), Satınalma Teklifi |
| **Stok (Inventory)** | Stok Girişi (Goods Receipt), Stok Çıkışı (Goods Issue), Depolar Arası Stok Transferi (Inventory Transfer) |
| **Finans (Banking)** | Tahsilat (Incoming Payments), Yapılan Ödeme (Outgoing Payments), Yevmiye Kaydı (Journal Entries), Dahili Mutabakatlar |
| **Üretim & Taslak** | Üretim Siparişi (Production Orders), Taslak Belgeler (Drafts) |

---

## 💻 Kullanılan Teknolojiler

- **Platform:** C#, .NET Framework / .NET Core, Windows Forms, Modern Flat UI
- **SAP Entegrasyonu:** SAP Business One Service Layer (OData REST) ve DI API (COM Entegrasyonu)
- **Veri & Çıktı:** Excel / ClosedXML, LINQ to Objects, Yapılandırılmış İşlem Loglama (Serilog)

---

## 🔒 Güvenlik ve Gizlilik Bildirimi
Uygulama kaynak kodları, şirket ve müşteri veritabanı bağlantı şifreleri bu depoda yer almaz. Ekran görüntüleri test ortamındaki örnek kurmaca verilerle üretilmiştir.
