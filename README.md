#  WhatsApp Message Scheduler & Professional Communication Assistant

Bu projeyi; staj başvuruları, iş görüşmeleri ve vakıf yazışmaları gibi profesyonel iletişim süreçlerimi daha verimli yönetmek için geliştirdim. Temel amacım, kurumsal nezaket kuralları ile otomasyonu birleştirerek iletişim kalitesini artırmaktır.

Akşam saatlerinde hazırladığım mesajların, belirlenen mesai saatleri içerisinde otomatik olarak iletilmesini sağlayarak profesyonel bir iş akışı oluşturuyorum.

##  Temel Özellikler
- **Mesaj Planlama:** İleri tarihli mesajlarımı SQL Server veritabanında güvenli bir şekilde saklıyorum.
- **Akıllı Zaman Yönetimi:** Kurumsal etik gereği 08:00 - 17:00 saatlerini baz alıyorum. Mesai dışı planladığım mesajlarda sistemin beni uyarmasını sağlıyorum.
- **Otomatik Gönderim:** Python motoru kullanarak, vakti gelen mesajların WhatsApp üzerinden iletilmesini sağlıyorum.
- **Gönderim Takibi:** Mesajların başarıyla iletilip iletilmediğini veritabanı üzerinden anlık olarak izliyorum.

##  Kullanım Senaryoları (Use Cases)
Bu aracı sadece bir mesaj gönderici değil, profesyonel iletişim asistanım olarak kurguladım:
- **İş/Staj Takibi:** İK uzmanlarına sabah mesai başlangıcında ulaşarak başvurularımın görünürlüğünü artırmak.
- **Vakıf & Organizasyon İletişimi:** Hafta sonu hazırladığım rapor veya soruların, Pazartesi sabahı kurumsal nezaket sınırları içinde iletilmesi.
- **Unutkanlığa Karşı Önlem:** Gece aklıma gelen kritik soruları kaydedip, yanlış saatte bildirim gönderilmesini önleyerek doğru zamanda iletmek.

##  Teknolojik Altyapı
- **Dil:** Python 3.13
- **Veritabanı:** Microsoft SQL Server (T-SQL)
- **Kütüphaneler:** `pyodbc`, `pywhatkit`, `schedule`
- **IDE:** Visual Studio Code

##  Veritabanı Şeması
Mesajları, **WhatsAppDB** veritabanında aşağıdaki tablo yapısıyla tutuyorum:
- `ID`: Benzersiz kayıt numarası (Primary Key)
- `PhoneNumber`: Alıcı telefon numarası
- `MessageContent`: Mesaj metni
- `SendTime`: Planlanan gönderim zamanı
- `IsSent`: Gönderim durumu (0: Bekliyor, 1: Tamamlandı)

## 🛠️ Kurulum ve Çalıştırma
*(Proje geliştirme aşamasındadır. Tamamlandığında adımlar buraya eklenecektir.)*
