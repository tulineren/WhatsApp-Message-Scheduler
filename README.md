#  WhatsApp Message Scheduler

Bu proje, profesyonel iletişim süreçlerini (staj başvuruları, vakıf görüşmeleri vb.) daha verimli yönetmek amacıyla geliştirilmiş bir **mesaj planlama otomasyonudur**. 

Akşam saatlerinde hazırlanan mesajların, belirlenen mesai saatleri içerisinde otomatik olarak iletilmesini sağlar.

##  Özellikler
- **Mesaj Planlama:** İleri tarihli mesajları SQL Server veritabanına kaydeder.
- **Otomatik Gönderim:** Belirlenen vakit geldiğinde Python botu aracılığıyla mesajı WhatsApp üzerinden iletir.
- **Durum Takibi:** Gönderilen ve bekleyen mesajların takibi yapılır.

##  Kullanılan Teknolojiler
- **Dil:** Python 3.13
- **Veritabanı:** Microsoft SQL Server (T-SQL)
- **Kütüphaneler:** `pyodbc`, `pywhatkit`, `schedule`
- **IDE:** VS Code

##  Veritabanı Şeması
Proje kapsamında mesajlar aşağıdaki yapıda saklanmaktadır:
- `ID`: Benzersiz kayıt numarası
- `PhoneNumber`: Alıcı telefon numarası
- `MessageContent`: Mesaj metni
- `SendTime`: Planlanan gönderim zamanı
- `IsSent`: Gönderim durumu (0: Bekliyor, 1: Tamamlandı)

##  Kurulum ve Çalıştırma
(Proje tamamlandığında bu kısım güncellenecektir.)
