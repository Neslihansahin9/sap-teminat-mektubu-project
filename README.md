# sap-teminat-mektubu-project
Kullanılan Teknolojiler
Teminat Mektubu  Project
Kullanılan Teknolojiler
SAP ERP
ABAP
SAP FI Modülü
ALV Grid
Dialog Programming
BAPI
Custom Z Tables
Selection Screen
Function Module
Object-Oriented ABAP
Proje Modülleri
1. Teminat Mektubu Programı

Teminat mektubu ana programı, kullanıcıların alınan ve verilen teminat mektuplarını yönetebilmesi amacıyla geliştirilmiştir. Program içerisinde belge oluşturma, belge görüntüleme, iade işlemi, vade değişikliği, dosya yükleme, belge yazdırma ve komisyon ekranına geçiş gibi işlemler bulunmaktadır.

Bu programda kullanıcı seçim ekranı üzerinden işlem türünü belirlemekte ve seçilen işleme göre ilgili ekranlara yönlendirilmektedir.

2. Teminat Mektubu Raporu

Rapor programı, sistemde kayıtlı teminat mektubu bilgilerinin belirli filtrelere göre listelenmesini sağlamaktadır. Şirket kodu, belge türü, özel defteri kebir göstergesi, müşteri, satıcı, açılış tarihi, vade tarihi, ürün ve referans numarası gibi kriterlerle raporlama yapılabilmektedir.

Rapor ekranında ALV yapısı kullanılmıştır. Bu sayede kullanıcılar kayıtları tablo formatında görüntüleyebilmekte, filtreleyebilmekte ve analiz edebilmektedir.

3. Komisyon Programı

Komisyon programı, teminat mektuplarına ait komisyon kayıtlarının takip edilmesi ve muhasebeleştirilmesi için geliştirilmiştir. Kullanıcılar banka, şirket kodu, tarih ve yıl bilgilerine göre komisyon kayıtlarını listeleyebilmekte ve seçilen kayıtlar için muhasebe belgesi oluşturabilmektedir.

Temel Fonksiyonlar
Teminat mektubu kaydı oluşturma
Müşteri ve satıcı bazlı teminat takibi
Vade değişikliği işlemleri
Komisyon hesaplama ve kayıt oluşturma
FI muhasebe belgesi oluşturma
Ters kayıt işlemleri
Belge görüntüleme
ALV raporlama
F4 arama yardımı
Kur çevrimi
Kullanıcı giriş kontrolleri
Kullanılan Önemli SAP Yapıları

Projede SAP FI modülü ile entegrasyon sağlamak amacıyla çeşitli standart SAP yapıları kullanılmıştır.

BAPI_ACC_DOCUMENT_POST

Muhasebe belgesi oluşturmak amacıyla kullanılmıştır. Teminat mektubu ve komisyon işlemlerinde belge başlığı, müşteri/satıcı kalemleri, ana hesap kalemleri ve tutar bilgileri doldurularak FI belgesi oluşturulmaktadır.

BAPI_ACC_DOCUMENT_REV_POST

Oluşturulan muhasebe belgelerinin ters kayıt işlemlerinde kullanılmıştır. İade veya iptal süreçlerinde önceki belgeye bağlı ters kayıt belgesi oluşturulmaktadır.

BAPI_TRANSACTION_COMMIT / BAPI_TRANSACTION_ROLLBACK

Belge oluşturma işleminin başarılı olması durumunda kayıtların sisteme kalıcı olarak işlenmesi için commit; hata oluşması durumunda işlemin geri alınması için rollback yapısı kullanılmıştır.

ALV Grid

Raporlama ekranlarında kullanıcıya tablo formatında veri sunmak amacıyla ALV Grid yapısı kullanılmıştır. Bu yapı sayesinde kullanıcılar teminat ve komisyon kayıtlarını daha okunabilir ve analiz edilebilir şekilde görüntüleyebilmektedir.

Custom Z Tables

Projede teminat mektubu ve komisyon süreçlerine ait verilerin saklanması için özel Z tablolar kullanılmıştır. Bu tablolar sayesinde standart SAP yapısında bulunmayan kuruma özel alanlar ve süreç bilgileri takip edilebilmektedir.

Proje Kapsamı

Bu proje, SAP FI modülü ile entegre çalışan özel bir teminat mektubu yönetim uygulamasıdır. Uygulama, işletmelerin teminat mektubu süreçlerini merkezi bir sistem üzerinden yönetmesine katkı sağlamaktadır. Geliştirilen yapı ile manuel takip süreçlerinin azaltılması, kullanıcı hatalarının önlenmesi, belge takibinin kolaylaştırılması ve finansal süreçlerin daha kontrollü yürütülmesi amaçlanmıştır.
