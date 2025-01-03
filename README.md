# Abap1
1
Yeni Program Oluşturma:
SAP'de SE38 veya SE80 işlem kodunu açın
"Create Program" (Program Oluştur) seçeneğini seçin
Program adını girin (örneğin: Z_OGRENCI_LISTESI)
Z veya Y ile başlamalı (müşteri namespace'i)
İsim 30 karakterden uzun olmamalı
Program türünü "Executable Program" (Çalıştırılabilir Program) olarak seçin

2
Metin Elementlerini Ekleme:
SE91 işlem kodunu kullanarak
Aşağıdaki metin elementini eklemelisiniz:
   TEXT-001 'Öğrenci Arama Kriterleri'

3
Bu basit program için INCLUDE'a gerek yok
Ancak büyük projelerde kodunuzu şu şekilde organize edebilirsiniz:
INCLUDE Z_OGRENCI_LISTESI_TOP.  " Global değişkenler ve yapılar
   INCLUDE Z_OGRENCI_LISTESI_SCR.  " Seçim ekranı
   INCLUDE Z_OGRENCI_LISTESI_F01.  " Alt programlar/fonksiyonlar

4
rogramı Kaydetme ve Aktive Etme:
Kodu yazdıktan sonra kaydedin (Ctrl + S)
Programı aktive edin (Ctrl + F3)
Herhangi bir syntax hatası varsa düzeltin

5Programı Test Etme:
F8 tuşuna basarak veya araç çubuğundaki "Execute" butonunu kullanarak programı çalıştırın
Test verilerinizle programı deneyin:
Önce öğrenci numarası ile arama yapın
Sonra ad/soyad ile arama yapın
Son olarak boş kriterlerde tüm listeyi görüntüleyin

Hata Ayıklama (Debug):
Programda hata olursa:
/h komutunu kullanarak debug moduna geçebilirsiniz
Değişkenlerin değerlerini kontrol edebilirsiniz
Kod akışını adım adım izleyebilirsiniz





