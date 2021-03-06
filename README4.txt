
.Net platformu ORM(Object Relational Mapping) araçlarından birisidir. 
ORM (Object Relational Mapping) ise veritabanı ile nesneye yönelik programlama (OOP) arasındaki ilişkiyi kuran teknolojidir. 
Yani Entity Framework, nesne tabanlı programlamada veri tabanındaki tablolara uygun nesneler oluşturma tekniğidir.

Entity Framework ile 4 farklı yöntem ile proje geliştirilebilir. Bu yöntemler;
1.Model First (New Database)
2.Database First (Existing Database)
3.Code First (New Database)

Model First (Önce Model): Bu yöntemde Visual Studio üzerinde boş bir model dosyası (.edmx) eklenerek veri tabanı bu model üzerinde tasarlanır. 
Derleme adımında verilen script dosyasi ile veri tabanı oluşturulur.

Database First (Önce Veritabanı): Bu yöntemde hali hazırda var olan veritabanı projeye model dosyası ile bağlanır ve gerekli class’lar EF tarafından üretilir. 

Code First (Önce Kod — Yeni Veritabanı): Bu yöntemde classlar ve mapping kodları yazılımcı tarafından oluşturulur. 
Daha sonra veri tabanı bu class’lardan türetilir. Biz projemizde Code First yöntemini kullanmaktayız.

Kullanıcı Verileri aşağıda verilen yöntemler ile veri tabanında toplanır.

- Giriş Yap Alanı: Üye hatalı giriş yapması durumunda bilgileri veri tabanına kaydedilir.

- Şifremi Unuttum Butonu: Kullanıcının şifresi unutması halinde, şifre yenileme e-postası gönderilir 
ve yeni şifre eski şifresinin bulunduğu alan üzerine güncelleme yapılır.

- Kayıt Ol Alanı: Kullanıcı Sistem üzerindeki kısıtlamalardan kurtulmak için kayıt olarak bilgileri veri tabanına kaydedilir.

- Üniversite alanı İçerik Ekle Butonları: Bu buton sayesinde üyeler belirledikleri kategoride kaynak eklerler. 
Her eklenilen kaynak verileri ayrı ayrı veri tabanında tutulur. 

- Etkinlik alanı İçerik Ekle Butonu: Bu buton ise üyelerin etkinliği oluşturacağı başlık, açıklama, etkinlik broşürü, konum ve tarih bilgilerini içerir. 
Her eklenilen etkinlik verisi veri tabanında tutulur. 

- Kaynakların içerisinde bulunan Paylaş Butonu: Üyeler yorum yaptılarında bu yorumlar (varsa etiketlediği kişiler) veri tabanına kaydedilir.
