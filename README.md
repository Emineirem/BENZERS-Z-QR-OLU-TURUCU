
# 🎟️ Etkinlik Katılımcı QR Sistemi

Bu proje,ATA YAPAY ZEKA Topluluğunun zirve etkinliğinde katılımcılara benzersiz qr oluşturup yollamak için yapılmış olup, bir Google Sheets formundan alınan başvuru verilerini kullanarak:

1. ✅ Onaylanan katılımcılar için **QR kodları oluşturur**  
2. ✉️ Oluşturulan QR kodlarını **kişisel e-posta adreslerine otomatik gönderir**

### 📌 Kullanım Senaryosu

Etkinliğe başvuran katılımcıların verileri Google Form üzerinden toplanır. Başvurular Google Sheets'e işlenir. Sistem, yalnızca "Onay Durumu" sütunu **EVET** olan kişilere QR kod gönderir.

---

## 🔧 Kurulum

### Gereksinimler
bash
pip install gspread oauth2client qrcode

#DOSYA YAPISI
├── qr_olustur.py           # QR kodları oluşturan script
├── qr_mail_gonder.py       # Mail gönderimini gerçekleştiren script
├── qr-service-key.json     # Google API erişimi için servis hesabı anahtarı
├── failed_sends.txt        # Hatalı gönderilen e-posta raporu
├── qr_ad_soyad.png         # Oluşturulan QR kodları (örnek dosyalar)
