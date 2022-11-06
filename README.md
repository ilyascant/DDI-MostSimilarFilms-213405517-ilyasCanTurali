### Daha iyi film onerisi almak icin yeni parametreler olustdurdum.

| Parametreler | ESKI ALGORITMA | YENI ALGORITMA |
| ------------ | :----------------: | :--------------: |
| Ozet Listesindeki Kelimeler | :heavy_check_mark: | :heavy_check_mark: (x4 Agirlik) |
| Oyuncular | :x: | :heavy_check_mark: (x1 Agirlik)  |
| Film Turleri | :x: | :heavy_check_mark: (x6 Agirlik) |
| Yonetmenler | :x: | :heavy_check_mark: (x2 Agirlik) |
> Oyuncular, Film Turleri ve Yonetmenler eklendi Sonuclara farkli etkiler etmeleri icin __agirliklar__ atadi.




### Yukaridaki katsayi isleminin kodu YENI ALGORITMA vs ESKI ALGORITMA
![resim](https://user-images.githubusercontent.com/79863003/200186623-2e8aadaa-e032-46e9-a6a0-0f4450da5385.png)

### Oyuncular, Film Turleri ve Yonetmenler veri tablosunda String olarak verildigi icin orn: "['Eddie Redmayne', 'Jude Law', 'Mads Mikkelsen']" ("[]") , ("'") isaretlerini kaldirip, (", ") virguler gore listelere ayirdim 
![resim](https://user-images.githubusercontent.com/79863003/200187245-65414007-e0de-4300-b79f-c387fec6febc.png)
````
clean_oyuncu = oyuncular.strip("[]").replace("'","").split(", ")
````


## Aranan Film 'Kirpi Sonic 2' , 50 Adet
![resim](https://user-images.githubusercontent.com/79863003/200185144-095c06a8-0ded-43ec-ac07-4f434dd6ed29.png)
> Resimde goruldugu gibi fazla arama sonuclari yapildiginda _ESKI ALGORITMADA_ tek parametre kullandigi icin aranan filmden bagimsiz onerilerde bulunabiliyor.
Orn: resimdeki goruldugu gibi _ESKI ALGORITMADA_ 39. ve 43 Onerilerde __Kirpi Sonic 2__ den bagimsiz _KORKU_ filmleri onermis.
ayni film icin __YENI ALGORITMADA__ ANIMASYON VE AILE_ filmleri onermeye devam etmistir.



#### Soldaki ilk 50 film onerisi _YENI ALGORITMA_  | Sagdaki ilk 50 film onerisi _ESKI ALGORITMA_
| YENI ALGORITMA   | ESKI ALGORITMA |
| ------------- | ------------- |
| Kirpi Sonic | Kirpi Sonic |
| İnanılmaz Aile 2 | Kirpi Latte ve Büyülü Taş |
| Küçük Denizkızı Ponyo | Dragon Rider |
| Ejderhanı Nasıl Eğitirsin 2 | Yapay Zeka |
| Robotlar | Alfa ve Omega: Eve Dönüş Macerası |
| Doğal Kahramanlar | İnanılmaz Aile 2 |
| Robinson Crusoe | Arabalar 3 |
| Altın Gol | Paw Patrol Filmi |
| Kutup Ekspresi | Zeko İçin |
| Korsanlar! | Uçan Halı ve Kayıp Elmas |
| Ainbo | Canım Kardeşim |
| Snoopy ve Charlie Brown Peanuts Filmi | Benimle Kal |
| Atlantis: Kayıp İmparatorluk | Tekken |
| Asteriks: Sihirli İksirin Sırrı | 9 |
| Dinozor | Doktor Strange: Çoklu Evren Çılgınlığında |
| Dinozor | Vikingler Büyük Macera |
| Rio | Karlar Kraliçesi 2 |
| Özgür Ruh | Karabasan |
| Orman Çocuğu 2 | Rüzgar |
| Efsane Beşli | Kimsesiz Çocuk Remi |
| Arı Maya 3 | Komando Dadı |
| Anastasia | Oda |
| Orman Çocuk | The Breed |
| Aslan: Hürkuş Kayıp Elmas | Uzay Yolu |
| Ejderhanı Nasıl Eğitirsin: Gizli Dünya | Kağıttan Kentler |
| Spirit: Özgür Ruh | Beverly Hills Çuvava |
| Aslan Kral | Sar Başa |
| Tinker Bell ve Korsan Peri | Tatlı Bela |
| Ejderhanı Nasıl Eğitirsin | Adventures of Shark Boy & Lava Girl in 3-D, The |
| Bay Peabody ve Meraklı Sherman: Zamanda Yolculuk | Ayı Teddy 2 |
| Paw Patrol Filmi | Lal |
| Tarzan | Ayas |
| Alvin ve Sincaplar: Yol Macerası | Ölüm Fısıltısı |
| Ayı Kardeş | İnanılmaz Aile |
| Garfield 2 | Looney Tunes: Maceraya Devam |
| Crood'lar | Alvin ve Sincaplar: Yol Macerası |
| Kuşlar Şehrinde Macera | Kesik |
| Kuzular Firarda | Dönerse Senindir |
| Crood'lar 2: Yeni Bir Çağ | The Human Centipede |
| Bolt | Şarkını Söyle |
| Horton | Astro Boy |
| Lego Batman Filmi | 9 |
| Kocaayak ve Ailesi | The Amityville Horror |
| Şrek 2 | Jurassic World: Hakimiyet |
| Garfield | Belle |
| Bay Link: Kayıp Efsane | Her Şey Her Yerde Aynı Anda |
| Oyunbozan Ralph | Man of Steel |
| Oyuncak Hikayesi 4 | İntihar Dükkanı |
| Dragon Rider | Bebe Şehirde |
| Kung Fu Panda 3 | Ayı Kardeş |


