# Leishmania Proteinleri
#### (Dosyalar açýklamalarýyla beraber aþaðýdadýr)
## Özet
Leishmania son derece ölümcül ve yaygýn bir hastalýktýr ve durdurulmalýdýr.
## Amaç
Leishmania parazitlerinin sahip olduðu önemli proteinlerden bir kaçýnýn yapýsýyla ilgili bir veri tabaný oluþturmak.

## Sonuçlar
Leishmania Mexicana, Leishmania Infantum ve Leishmania Braziliansis parazitlerinin sahip olduðu bir takým proteinler hakkýnda yeni modeller ve grafikler çýkardýk.
### Bir takým tablolamalarda kullanýlabilecek format
| Leishmania Mexicana | Leishmania Infantum         | Leishmania Braziliansis     |
|-------------------  |-----------------------------|-----------------------------|
|### [Model1](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Deneysel_veriseti.csv)| 1                           | 1                           |
| 2                   | 2                           | 2                           |

## Kullandýðýmýz Dosyalar
### [Deneysel Veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Deneysel_veriseti.csv)
SARS-CoV-2’nin S-proteininindeki Hedef Tanýma Modülü (HTM) bölgesindeki olasý tüm nokta mutasyonlarýn ACE2 proteinine baðlanmasý üzerindeki etkilerini gösteren deneysel veriseti.
### [Özellikler](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Ozellikler.csv)
Her bir aminoaside ait hidropati indeksi ve moleküler kütleyi gösteren veriseti. Kullandýðýmýz verisetlerini oluþtururken buradaki özelliklerden yararlandýk.
###  [Veri Düzenleme Jupyter Notebook](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Veri%20Duzenleme%202.ipynb) | [Veri Düzenleme Python Script](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriduzenleme.py)
Varolan bazý verisetlerinden aldýðýmýz veriyi bu kodla birleþtirip ve düzenleyip verisetlerimizi oluþturduk. Python script ve Jupyter Notebook formatlarýnda kodu inceleyebilirsiniz.
### [Veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti.csv)
Kodumuzdaki veriyial() fonksiyonu ile oluþturduðumuz, hedef tanýma modülü'ndeki bütün mutasyonlarý ve bu mutasyonlarýn hidropati farký, moleküler kütle farký, baðlanma ortalamasý, ekspresyon ortalamasý, polarite farký ve hacim farký özelliklerini bulunduran veriseti. Farklarý hesaplarken mutant aminoaside ait olan özelliði vahþitip aminoasidinden çýkardýk.
### [Veriseti Baðlanma Sýfýr ve Üstü](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti_baglanma_sifir_ve_ustu)
[veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti.csv) dosyasýndaki baðlanma afinitesi (bind_avg) deðeri sýfýra eþit veya sýfýrdan büyük olan mutasyonlarý içermektedir. Bu verisetini oluþturmak için kodumuzdaki baglanmasifirveustu() fonksiyonu ile baðlanma deðeri sýfýra eþit olan veya sýfýrdan büyük olan mutasyonlarý seçtik.
### [Veriseti Yeni Özellikler](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti_yeni_ozellikler) 
[veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti.csv) dosyasýna kodumuzdaki yeniozellikekle() fonksiyonuyla halka sayýsý farký, hidrojen atomu sayýsý farký, oksijen atomu sayýsý farký, çift bað sayýsý farký özelliklerini ekledik.
### [Veriseti Yeni Özellikler Baðlanma Sýfýr ve Üstü](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Veriseti_Yeni_Ozellikler_Baglanma_Sifir_ve_Ustu.csv)
[Veriseti Yeni Özellikler](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti_yeni_ozellikler) dosyasýndaki baðlanma deðeri (bind_avg) sýfýr ve üstü olan mutasyonlarý seçtiðimiz veriseti. Bu verisetini oluþturmak için baglanmasýfýrveustu() fonksiyonunu kullandýk.

# 2.Etap Analiz
2.Analizde mutasyon yerine interaksiyonlarý inceledik. Star ve Arkadaþlarýnýn oluþturmuþ olduðu RBD-ACE2 ikili interaksiyon verisi Python kodunda iþleyerek çoklu interaksiyon verisi haline getirdik. Bu analizde probleme farklý bir açýdan yaklaþmýþ olup, sadece RBD'yi deðil, RBD ve ACE2'yi beraber inceleyerek daha bütünsel bir analiz yapmýþ olduk.  

## K-Means Analiz Grafiði
| Küme Sayýsý | Küme 0 Eleman Sayýsý          | Küme 1 Eleman Sayýsý  | Küme 2 Eleman Sayýsý | Küme 3 Eleman Sayýsý  | Küme 4 Eleman Sayýsý | Küme 5 Eleman Sayýsý | Küme 6 Eleman Sayýsý |
|-------------|-------------------------------|-----------------------|----------------------|-----------------------|----------------------|----------------------|----------------------|
| 2           | 11(%52, K417 ve K484 burada)  | 10 (%48, Y501 burada) | 0                    | 0                     | 0                    | 0                    | 0                    |
| 3           | 7 (%33,  K417 ve K484 burada) | 6 (%29)               | 8 (%38, Y501 burada) | 0                     | 0                    | 0                    | 0                    |
| 4           | 5 (%24, 484K burada)          | 3 (%14)               | 8 (%38, 501Y burada) | 8 (%38, 501Y burada)  | 0                    | 0                    | 0                    |
| 5           | 3 ( %14, K484 burada)         | 5 (%24)               | 2 (%10)              | 3 (%14, K417 burada)  | 8 (%38, Y501 burada) | 0                    | 0                    |
| 6           | 3 (% 14, 484K burada)         | 5 (%24)               | 2 (%10)              | 3 (%14, K417 burada)  | 4 (%19)              | 4 (%19, 501Y burada) | 0                    |
| 7           | 3 (% 14, K484 burada)         | 5 (%24)               | 2 (%10)              | 2 (%10)               | 4 (%19)              | 4 (%19, 501Y burada) | 1 (%5, K417 burada)  |

## Dosyalar
### [ACE2-RBD Ýnteraksiyon Verisi](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/ACE2-RBD_contact_details.txt)
ACE2 ve RBD tekli interaksiyon verisi içerir. Python kodumuzda, bir önceki analizimizdeki elde ettiðimiz özellik listesiyle birleþtirdik, tekli interaksiyon verisinden çoklu interaksiyon verisine çevirdik ve analize hazýr hale getirdik.
### [Açýklamalý Veri Düzenleme Kodu](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Veri_D%C3%BCzenleme.ipynb) 
Veriyi Weka'da düzenlemeye uygun hale getirmek için kullandýðýmýz Jupyter Notebook. Veri üstüne yaptýðýmýz iþlemlerin kodlarý açýklamalarýyla beraber burada.
### [Çoklu Ýnteraksiyon Verisi](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/%C3%87oklu%20%C4%B0nteraksiyon.csv)
Açýklamalý veri düzenleme kodu kullanýlarak hazýradýðýmýz, verinin analizinde kullandýðýmýz son halidir.
