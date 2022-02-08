# Leishmania Proteinleri
#### (Dosyalar a��klamalar�yla beraber a�a��dad�r)
## �zet
2019 y�l�nda ortaya ��kan ve 223 �lkeyi etkisi alt�nda alan COVID-19 pandemisi, g�n�m�ze (Eyl�l 2021) kadar 221 milyon vakaya ve 4.6 milyon �l�me sebep olmu�tur (WHO, 2021). COVID-19 pandemisi, SARS-CoV-2 vir�s�n�n ve bu vir�se avantaj sa�layan varyantlar�n�n h�zla yay�lmas� sonucunda bu bula��c�l�k seviyesine eri�mi�tir. Bahsi ge�en avantaj sa�lay�c� varyantlar, �zellikle tek amino asit (nokta) baz�nda g�r�len mutasyonlar yoluyla meydana gelmi�tir. Bu nokta mutasyonlar�, SARS-CoV-2�nin yap�s�nda de�i�ikliklere yol a�abildi�i gibi, vir�s�n insan kona��na girmek i�in ilk basamak olarak kulland��� ACE2 proteini ile etkile�im verimini de etkileyebilmektedir. ACE2 ile ba�lanmay� etkileyen N501Y ve E484K mutasyonlar� yayg�n olarak �ngiltere�de, G�ney Afrika�da ve Brezilya�da g�zlemlenmi� ve t�m d�nyada endi�eye sebep olmu�tur. Bu olgudan yola ��karak tasarlad���m�z projede, N501Y ve E484K kadar etkin olabilecek ve bula��c�l���n�n y�ksek olmas� nedeniyle tehlike yaratabilecek SARS-CoV-2 mutasyonlar�n�n tahmin edilmesi ama�land�. Bu hedef do�rultusunda, �zg�n bir �al��ma olarak, SARS-CoV-2 ve ACE2 ba�lanma ve stabilitesine ait deneysel veriler farkl� aminoasit �zellikleri ile ili�kilendirilip, makine ��renmesi ve hesaplamal� biyoloji tekniklerine entegre ederek, algoritmalarda yap�lan analizler sonucunda _**N501M, Q414A, N354K, Q498H, N460K, N501W**_ mutasyonlar�n�n, koronavir�s�n�n yay�lmas�nda tehlikeli olma ihtimallerinin y�ksek oldu�u belirlendi. �u anda yayg�n olan varyantlardan birinde g�r�len 501. pozisyon mutasyonlar�na �zellikle dikkat edilmesi gerekti�ini, bu pozisyonunun listelerde tekrar etmesi �zerine �zellikle �nermekteyiz. �zellikle sekanslama s�ras�nda kar��la��lmas� durumunda bu mutasyonlar�n yay�l�m�n�n engellenmesi konusunda b�y�k hassasiyet g�sterilmeli ve gerekli sa�l�k tedbirleri al�nmal�d�r. Makine ��renmesi ve hesaplamal� biyoloji �����nda yap�lan bu ara�t�rman�n sonu�lar� COVID-19 pandemisi konusunda ileriki �al��malara alt yap� sa�layacak ve vir�sle olan sava�ta bilim insanlar�na yol g�sterecektir. 

## Ama�
Leishmania parazitlerinin sahip oldu�u �nemli proteinlerden bir ka��n�n yap�s�yla ilgili bir veri taban� olu�turmak.

## Sonu�lar
Leishmania Mexicana, Leishmania Infantum ve Leishmania Braziliansis parazitlerinin sahip oldu�u bir tak�m proteinler hakk�nda yeni modeller ve grafikler ��kard�k.
### Bir tak�m tablolamalarda kullan�labilecek format
| Bir tak�m veriler | Bir tak�m veriler | Bir tak�m veriler |Bir tak�m veriler | Bir tak�m veriler |
|----------------|-----------------------------|-----------------------------|------------------------------------------------|------------------------------------------------|
| 2              | 1                           | 1                           | 445                                            | 445                                            |
| 3              | 1                           | 1                           | 299                                            | 299                                            |
| 4              | 3                           | 3                           | 164                                            | 164                                            |
| 5              | 3                           | 3                           | 164                                            | 164                                            |
| 6              | 5                           | 3                           | 118                                            | 66                                             |
| 7              | 5                           | 3                           | 119                                            | 65                                             |
| 8              | 1                           | 1                           | 57                                             | 57                                             |
| 9              | 8                           | 8                           | 56                                             | 56                                             |
| 10             | 9                           | 9                           | 30                                             | 30                                             |
| 11             | 9                           | 9                           | 30                                             | 30                                             |
| 12             | 9                           | 9                           | 29                                             | 29                                             |

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
