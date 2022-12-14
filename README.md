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
### Oyuncular arasinda "NONE" isimli oyuncular vardi onlari islemlere katmamak icin NONE gorulen yerlerde matrix degerini +1 yapmak yerine o islemi iptal ettim.
![resim](https://user-images.githubusercontent.com/79863003/200187530-2e01ada8-ae28-4641-bed9-266bedd6dde7.png)
![resim](https://user-images.githubusercontent.com/79863003/200187466-e4244cdd-59c3-44b1-9009-45de3b1c6ac5.png)


## Aranan Film 'Kirpi Sonic 2' , 50 Adet
![resim](https://user-images.githubusercontent.com/79863003/200185144-095c06a8-0ded-43ec-ac07-4f434dd6ed29.png)
> Resimde goruldugu gibi fazla arama sonuclari yapildiginda _ESKI ALGORITMADA_ tek parametre kullandigi icin aranan filmden bagimsiz onerilerde bulunabiliyor.
Orn: resimdeki goruldugu gibi _ESKI ALGORITMADA_ 39. ve 43 Onerilerde __Kirpi Sonic 2__ den bagimsiz _KORKU_ filmleri onermis.
ayni film icin __YENI ALGORITMADA__ _ANIMASYON VE AILE_ filmleri onermeye devam etmistir.



#### Soldaki ilk 50 film onerisi _YENI ALGORITMA_  | Sagdaki ilk 50 film onerisi _ESKI ALGORITMA_
| YENI ALGORITMA   | ESKI ALGORITMA |
| ------------- | ------------- |
| Kirpi Sonic | Kirpi Sonic |
| ??nan??lmaz Aile 2 | Kirpi Latte ve B??y??l?? Ta?? |
| K??????k Denizk??z?? Ponyo | Dragon Rider |
| Ejderhan?? Nas??l E??itirsin 2 | Yapay Zeka |
| Robotlar | Alfa ve Omega: Eve D??n???? Maceras?? |
| Do??al Kahramanlar | ??nan??lmaz Aile 2 |
| Robinson Crusoe | Arabalar 3 |
| Alt??n Gol | Paw Patrol Filmi |
| Kutup Ekspresi | Zeko ????in |
| Korsanlar! | U??an Hal?? ve Kay??p Elmas |
| Ainbo | Can??m Karde??im |
| Snoopy ve Charlie Brown Peanuts Filmi | Benimle Kal |
| Atlantis: Kay??p ??mparatorluk | Tekken |
| Asteriks: Sihirli ??ksirin S??rr?? | 9 |
| Dinozor | Doktor Strange: ??oklu Evren ????lg??nl??????nda |
| Dinozor | Vikingler B??y??k Macera |
| Rio | Karlar Krali??esi 2 |
| ??zg??r Ruh | Karabasan |
| Orman ??ocu??u 2 | R??zgar |
| Efsane Be??li | Kimsesiz ??ocuk Remi |
| Ar?? Maya 3 | Komando Dad?? |
| Anastasia | Oda |
| Orman ??ocuk | The Breed |
| Aslan: H??rku?? Kay??p Elmas | Uzay Yolu |
| Ejderhan?? Nas??l E??itirsin: Gizli D??nya | Ka????ttan Kentler |
| Spirit: ??zg??r Ruh | Beverly Hills ??uvava |
| Aslan Kral | Sar Ba??a |
| Tinker Bell ve Korsan Peri | Tatl?? Bela |
| Ejderhan?? Nas??l E??itirsin | Adventures of Shark Boy & Lava Girl in 3-D, The |
| Bay Peabody ve Merakl?? Sherman: Zamanda Yolculuk | Ay?? Teddy 2 |
| Paw Patrol Filmi | Lal |
| Tarzan | Ayas |
| Alvin ve Sincaplar: Yol Maceras?? | ??l??m F??s??lt??s?? |
| Ay?? Karde?? | ??nan??lmaz Aile |
| Garfield 2 | Looney Tunes: Maceraya Devam |
| Crood'lar | Alvin ve Sincaplar: Yol Maceras?? |
| Ku??lar ??ehrinde Macera | Kesik |
| Kuzular Firarda | D??nerse Senindir |
| Crood'lar 2: Yeni Bir ??a?? | The Human Centipede |
| Bolt | ??ark??n?? S??yle |
| Horton | Astro Boy |
| Lego Batman Filmi | 9 |
| Kocaayak ve Ailesi | The Amityville Horror |
| ??rek 2 | Jurassic World: Hakimiyet |
| Garfield | Belle |
| Bay Link: Kay??p Efsane | Her ??ey Her Yerde Ayn?? Anda |
| Oyunbozan Ralph | Man of Steel |
| Oyuncak Hikayesi 4 | ??ntihar D??kkan?? |
| Dragon Rider | Bebe ??ehirde |
| Kung Fu Panda 3 | Ay?? Karde?? |


