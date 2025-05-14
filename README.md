# 🚀 Web Application Firewall (WAF)

Web Application Firewall (WAF), web uygulamalarınızı yaygın saldırılara karşı korumak için geliştirilmiş hafif ve güçlü bir güvenlik çözümüdür. Bu proje, 24 saatlik bir Hackathon etkinliğinde sıfırdan geliştirilmiştir.

---

## 🛡️ Özellikler
- SQL Injection tespiti ve engelleme
- XSS (Cross-Site Scripting) saldırı tespiti
- Basit DoS koruması (istek limiti)
- Saldırı kayıtlarının veritabanında tutulması
- Kullanıcı girişi ve oturum yönetimi
- Modern ve sade arayüz

---

## ⚙️ Kurulum

1. **Python Sanal Ortamı Oluşturun**
    ```bash
    python -m venv venv
    source venv/bin/activate  # (Windows için: venv\Scripts\activate)
    ```
2. **Gerekli Paketleri Yükleyin**
    ```bash
    pip install -r requirements.txt
    ```
3. **Sunucuyu Başlatın**
    ```bash
    python Server.py
    ```
    Sunucu varsayılan olarak [http://localhost:5000](http://localhost:5000) adresinde çalışır.

---

## 🗄️ Veritabanı Kontrolü
- Veritabanı: `waf.db` (SQLite)
- Saldırı kayıtlarını görmek için:
    ```bash
    sqlite3 waf.db
    SELECT * FROM attacks;
    ```

---

## 📁 Proje Yapısı
```
├── Server.py           # Ana sunucu ve uygulama dosyası
├── AttackTest.py       # Saldırı tespit ve loglama
├── SQLi.py             # SQL Injection tespiti
├── XSS.py              # XSS tespiti
├── DOS.py              # DoS koruması
├── requirements.txt    # Gerekli Python paketleri
├── Templates/          # HTML şablonları
└── README.md           # Proje dokümantasyonu
```

---

## 📸 Ekran Görüntüsü
> **Not:** Arayüz ve saldırı kayıtları için ekran görüntüsü ekleyebilirsiniz.

---

## 📬 Katkı ve İletişim
Her türlü katkı ve geri bildirime açıktır. Lütfen issue veya pull request açmaktan çekinmeyin!