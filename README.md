# Leishmania Proteinleri
#### (Dosyalar a��klamalar�yla beraber a�a��dad�r)
## �zet
Leishmania son derece �l�mc�l ve yayg�n bir hastal�kt�r ve durdurulmal�d�r.
## Ama�
Leishmania parazitlerinin sahip oldu�u �nemli proteinlerden bir ka��n�n yap�s�yla ilgili bir veri taban� olu�turmak.

## Sonu�lar
Leishmania Mexicana, Leishmania Infantum ve Leishmania Braziliansis parazitlerinin sahip oldu�u bir tak�m proteinler hakk�nda yeni modeller ve grafikler ��kard�k.
### Bir tak�m tablolamalarda kullan�labilecek format
| Leishmania Mexicana | Leishmania Infantum         | Leishmania Braziliansis     |
|-------------------  |-----------------------------|-----------------------------|
|### [Model1](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Deneysel_veriseti.csv)| 1                           | 1                           |
| 2                   | 2                           | 2                           |

## Kulland���m�z Dosyalar
### [Deneysel Veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Deneysel_veriseti.csv)
SARS-CoV-2�nin S-proteininindeki Hedef Tan�ma Mod�l� (HTM) b�lgesindeki olas� t�m nokta mutasyonlar�n ACE2 proteinine ba�lanmas� �zerindeki etkilerini g�steren deneysel veriseti.
### [�zellikler](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Ozellikler.csv)
Her bir aminoaside ait hidropati indeksi ve molek�ler k�tleyi g�steren veriseti. Kulland���m�z verisetlerini olu�tururken buradaki �zelliklerden yararland�k.
###  [Veri D�zenleme Jupyter Notebook](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Veri%20Duzenleme%202.ipynb) | [Veri D�zenleme Python Script](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriduzenleme.py)
Varolan baz� verisetlerinden ald���m�z veriyi bu kodla birle�tirip ve d�zenleyip verisetlerimizi olu�turduk. Python script ve Jupyter Notebook formatlar�nda kodu inceleyebilirsiniz.
### [Veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti.csv)
Kodumuzdaki veriyial() fonksiyonu ile olu�turdu�umuz, hedef tan�ma mod�l�'ndeki b�t�n mutasyonlar� ve bu mutasyonlar�n hidropati fark�, molek�ler k�tle fark�, ba�lanma ortalamas�, ekspresyon ortalamas�, polarite fark� ve hacim fark� �zelliklerini bulunduran veriseti. Farklar� hesaplarken mutant aminoaside ait olan �zelli�i vah�itip aminoasidinden ��kard�k.
### [Veriseti Ba�lanma S�f�r ve �st�](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti_baglanma_sifir_ve_ustu)
[veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti.csv) dosyas�ndaki ba�lanma afinitesi (bind_avg) de�eri s�f�ra e�it veya s�f�rdan b�y�k olan mutasyonlar� i�ermektedir. Bu verisetini olu�turmak i�in kodumuzdaki baglanmasifirveustu() fonksiyonu ile ba�lanma de�eri s�f�ra e�it olan veya s�f�rdan b�y�k olan mutasyonlar� se�tik.
### [Veriseti Yeni �zellikler](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti_yeni_ozellikler) 
[veriseti](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti.csv) dosyas�na kodumuzdaki yeniozellikekle() fonksiyonuyla halka say�s� fark�, hidrojen atomu say�s� fark�, oksijen atomu say�s� fark�, �ift ba� say�s� fark� �zelliklerini ekledik.
### [Veriseti Yeni �zellikler Ba�lanma S�f�r ve �st�](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Veriseti_Yeni_Ozellikler_Baglanma_Sifir_ve_Ustu.csv)
[Veriseti Yeni �zellikler](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/veriseti_yeni_ozellikler) dosyas�ndaki ba�lanma de�eri (bind_avg) s�f�r ve �st� olan mutasyonlar� se�ti�imiz veriseti. Bu verisetini olu�turmak i�in baglanmas�f�rveustu() fonksiyonunu kulland�k.

# 2.Etap Analiz
2.Analizde mutasyon yerine interaksiyonlar� inceledik. Star ve Arkada�lar�n�n olu�turmu� oldu�u RBD-ACE2 ikili interaksiyon verisi Python kodunda i�leyerek �oklu interaksiyon verisi haline getirdik. Bu analizde probleme farkl� bir a��dan yakla�m�� olup, sadece RBD'yi de�il, RBD ve ACE2'yi beraber inceleyerek daha b�t�nsel bir analiz yapm�� olduk.  

## K-Means Analiz Grafi�i
| K�me Say�s� | K�me 0 Eleman Say�s�          | K�me 1 Eleman Say�s�  | K�me 2 Eleman Say�s� | K�me 3 Eleman Say�s�  | K�me 4 Eleman Say�s� | K�me 5 Eleman Say�s� | K�me 6 Eleman Say�s� |
|-------------|-------------------------------|-----------------------|----------------------|-----------------------|----------------------|----------------------|----------------------|
| 2           | 11(%52, K417 ve K484 burada)  | 10 (%48, Y501 burada) | 0                    | 0                     | 0                    | 0                    | 0                    |
| 3           | 7 (%33,  K417 ve K484 burada) | 6 (%29)               | 8 (%38, Y501 burada) | 0                     | 0                    | 0                    | 0                    |
| 4           | 5 (%24, 484K burada)          | 3 (%14)               | 8 (%38, 501Y burada) | 8 (%38, 501Y burada)  | 0                    | 0                    | 0                    |
| 5           | 3 ( %14, K484 burada)         | 5 (%24)               | 2 (%10)              | 3 (%14, K417 burada)  | 8 (%38, Y501 burada) | 0                    | 0                    |
| 6           | 3 (% 14, 484K burada)         | 5 (%24)               | 2 (%10)              | 3 (%14, K417 burada)  | 4 (%19)              | 4 (%19, 501Y burada) | 0                    |
| 7           | 3 (% 14, K484 burada)         | 5 (%24)               | 2 (%10)              | 2 (%10)               | 4 (%19)              | 4 (%19, 501Y burada) | 1 (%5, K417 burada)  |

## Dosyalar
### [ACE2-RBD �nteraksiyon Verisi](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/ACE2-RBD_contact_details.txt)
ACE2 ve RBD tekli interaksiyon verisi i�erir. Python kodumuzda, bir �nceki analizimizdeki elde etti�imiz �zellik listesiyle birle�tirdik, tekli interaksiyon verisinden �oklu interaksiyon verisine �evirdik ve analize haz�r hale getirdik.
### [A��klamal� Veri D�zenleme Kodu](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/Veri_D%C3%BCzenleme.ipynb) 
Veriyi Weka'da d�zenlemeye uygun hale getirmek i�in kulland���m�z Jupyter Notebook. Veri �st�ne yapt���m�z i�lemlerin kodlar� a��klamalar�yla beraber burada.
### [�oklu �nteraksiyon Verisi](https://github.com/BiyoinformatikProje/Bulasiciligi-Arttiran-Koronavirus-SARS-CoV-2-Mutasyonlarinin-Tahmini/blob/main/%C3%87oklu%20%C4%B0nteraksiyon.csv)
A��klamal� veri d�zenleme kodu kullan�larak haz�rad���m�z, verinin analizinde kulland���m�z son halidir.
