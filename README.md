# 🕷️ XSS Lab – Web Güvenlik Açığı Çalışmaları

Bu projede, Reflected ve Stored XSS açıkları üzerine örnekler, payload testleri ve çözümler yer almaktadır.

---

## 🔍 Amaç

XSS (Cross-site Scripting) açıklarının anlaşılması, örnek senaryolarla denenmesi ve manuel test pratiği kazanılması.

---

## 🧪 Reflected XSS Örnekleri

- `search?q=<script>alert('XSS')</script>`
- `<img src=x onerror=alert('XSS')>`
- `<svg/onload=alert(1)>`

---

## 🧠 Stored XSS Notları

- Yorum alanlarına `<script>` etiketleri girildiğinde tetiklenmesi
- Kalıcı olarak kaydedilip başka kullanıcıda çalışması

---

## 🧰 Kullanılan Araçlar

- Burp Suite
- OWASP Juice Shop
- DVWA (Damn Vulnerable Web App)
- Firefox + Add-on (HackBar)

---

## 🖼️ Ekran Görüntüleri

📂 `screenshots/` klasöründe örnek test çıktılarına yer verilmiştir.

---

## 📌 Notlar

Bu çalışma eğitim amaçlıdır. Gerçek sistemlerde izinsiz test yapmak suçtur.
