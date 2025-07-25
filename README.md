# 🛡️ XSS Lab – Web Güvenlik Açığı Testleri

Bu projede, Cross-Site Scripting (XSS) açıklarını anlamak ve test etmek amacıyla hazırladığım senaryolar, payloadlar ve örnekler yer almaktadır.

---

## 📚 XSS Nedir?

**XSS (Cross-Site Scripting)**, kötü niyetli bir kullanıcının web sayfasına JavaScript kodu enjekte etmesiyle kullanıcıyı hedef alan bir web güvenlik açığıdır. Üç ana türü vardır:

1. **Reflected XSS**
2. **Stored (Persistent) XSS**
3. **DOM-Based XSS**

---

## 🧪 Reflected XSS Örnekleri

- `https://hedefsite.com/search?q=<script>alert('XSS')</script>`
- `<img src=x onerror=alert('XSS')>`
- `<svg/onload=alert('Reflected XSS')>`

📝 Açıklama: Sunucuya gönderilen zararlı veri hemen geri yansıtılarak kullanıcı tarayıcısında çalışır.

---

## 🗃️ Stored XSS Örneği

- `<script>alert('Stored XSS')</script>`

📝 Açıklama: Zararlı içerik sunucuda saklanır, başka kullanıcılar sayfayı ziyaret ettiğinde tetiklenir.

---

## 🔁 DOM-Based XSS Örnekleri

- `<a href="javascript:alert('DOM XSS')">Tıkla</a>`
- `document.location = "javascript:alert('XSS')"`

📝 Açıklama: Tarayıcıda çalışan JavaScript kodları üzerinden gerçekleşir, sunucuya hiç gitmeyebilir.

---

## 🧰 Kullanılan Araçlar

- Burp Suite
- OWASP Juice Shop
- DVWA
- Firefox HackBar eklentisi
- Chrome Developer Tools

---

## 📂 Klasörler

| Klasör         | Açıklama                                 |
|----------------|-------------------------------------------|
| `payloads.txt` | Denediğim tüm XSS payloadlarının listesi |
| `screenshots/` | Ekran görüntüleri                        |
| `labs/`        | HTML açık örnek dosyaları (test için)    |
| `resources.md` | Kaynaklar ve referanslar                 |

---

## ⚠️ Etik Uyarı

> Bu proje yalnızca eğitim ve bilgi amaçlıdır. Gerçek sistemlerde izinsiz güvenlik testi yapmak **yasalara aykırıdır**.

---
![Reflected XSS PortSwigger](ekran%20g%C3%B6r%C3%BCnt%C3%BCleri/reflected-xss-portswigger.png)

