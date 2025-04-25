# Projektin avaaminen QFieldissa

GeoPackage-tiedostoon tallennettu QGIS-projekti avautuu QFieldissa suoriltaan ilman välivaiheita. GeoPackagen voi avata eri tavoilla, ml. lataamalla GeoPackage-tiedoston Android-mobiilipäätteelle, avaamalla tiedoston Google Drive -linkin tai Google Drive -sovelluksen kautta.

## Projektin avaaminen QFieldin *Tuo URL*-toiminnolla (helpoin)

1.  Avaa QField ja valitse *Avaa paikallinen tiedosto*.

2.  Klikkaa oikean alakulman + -painiketta ja valitse *Tuo URL*

3.  Liitä avautuvaan ikkunaan tämä ZIP-paketin suoraosoite:
    <https://drive.google.com/uc?export=download&id=1eDXXaWPuvdf8Gh_VLST9cFO6T7tb2N1N>

4.  Valitse *"Projektit"*- kohdasta projektitiedosto.

<video width="640" height="360" controls>

<source src="img/tuo_URL-osoitteesta_QField.mp4" type="video/mp4">

</video>

## Projektin avaaminen QFieldin *Tuo projekti ZIP-tiedostosta* toiminnolla (vaihtoehtoinen)

1.  Lataa [Google drive ZIP-tiedosto](https://drive.google.com/file/d/1eDXXaWPuvdf8Gh_VLST9cFO6T7tb2N1N/view?usp=sharing) puhelimeesi.

2.  Avaa QField ja valitse *Avaa paikallinen tiedosto*.

3.  Klikkaa oikean alakulman + -painiketta ja valitse *"Tuo projekti ZIP-tiedostosta"*

4.  Etsi juuri ladattu tiedosto. Löytyy yleensä Lataukset/Downloads- kansiosta.

5.  Jos QField löytää vanhan version, valitse *"Tuonti ja päällekirjoitus"*

6.  Valitse *"Projektit"*- kohdasta projektitiedosto.

<video width="640" height="360" controls>

<source src="img/projektin_avaus.mp4" type="video/mp4">

</video>

## Projektin avaaminen suoraan tiedostosta (ei suositeltu)

Ladattuasi tiedoston Andoid-mobiililaitteelle voit joko klikata GeoPackage-tiedoston auki tiedostonhallinnasta tai avata tiedoston QField-sovelluksen kautta. Tärkeää on, että ladattuasi tiedoston Android-laitteella tiedät, mistä löydät GeoPackage-tiedoston (esim. /Download-kansion sisältä).

Voit painaa Androidissa GeoPackage-tiedostoa ja laitteen pitäisi tunnistaa, että GeoPackage-tiedostotyyppi on yhteensopiva nimenomaan QField-sovelluksen kanssa ja avata se suoraan:

<video width="640" height="360" controls>

<source src="img/qfield_projektin_avaus_tiedostonhallinnasta.mp4" type="video/mp4">

</video>

Saattaa olla, että on helpompi avata projekti QField-sovelluksen kautta osoittaen sovelluksesta, missä projektitiedosto sijaitsee:

<video width="640" height="360" controls>

<source src="img/qfield_projektin_avaus_qfieldin_kautta.mp4" type="video/mp4">

</video>

## Projektin avaaminen Google Drive sähköposti-linkin avaulla (ei suositeltu)

Jos olet saanut Projektitiedoston jakoon Google Drive -kansion kautta, voit avata projektin myös sitä kautta:

1.  Avaa sähköpostisovellus puhelimellasi.
2.  Avaa sähköpostiisi tullut viesti, jossa ilmoitettaan että sinulle on jaettu kohde
3.  Paina viestin "Avaa"- painiketta Ensimmäisellä kerralla voi olla että sinulta kysytään varmistuskoodia, joka lähetettään sähköpostiisi. Syötä tämä sähköpostiisi lähetetty varmistuskoodi niin pääset jatkamaan.
4.  Lataa tiedosto "Lataa"-painikkeeen avulla.
5.  Kun tiedosto on ladattu, paina "Avaa" ja valitse sovellukseksi QField.
6.  QField sovellus aukeaa, jossa on projektitiedosto valmiiksi ladattuna.

<video width="640" height="360" controls>

<source src="img/qfield_projektin_avaus_spostista.mp4" type="video/mp4">

</video>

Voit myös hyödyntää Google Drive -sovellusta ja avata tiedoston sitä kautta:

1.  Avaa Google Drive- puhelimellasi
2.  Klikkaa GeoPackage -tiedostoa, joka on jaettu sinulle. (Yleensä näkyy heti aloitussivulla)
3.  Valitse sovellukseksi QField.
4.  QField sovellus aukeaa, jossa on projektitiedosto valmiiksi ladattuna.

<video width="640" height="360" controls>

<source src="img/qfield_projektin_avaus_drivesta.mp4" type="video/mp4">

</video>

## Projektin pakkaaminen ja vienti QFieldiin QFielSync-QGIS-lisäosan avulla

Jos sinun tarvitsee tehdä edistyneitä määrityksiä projektitiedostoon, sinun on hyödynnettävä QFieldSync-QGIS-lisäosaa ja paketoida QField-projekti sitä kautta erilliseen tiedostohakemistoon.

### Projektin pakkaaminen

QGIS-projekti viedään QFieldiin kopioimalla tarvittavat tiedostot sisältävä kansio tietokoneelta mobiililaitteelle. Ensin pitää kuitenkin tehdä pakkaaminen QField Sync-lisäosan kautta. Avaa **Pakkaa QFieldiä varten** "Package for QField" työkalupalkista

[<img src="img/qfieldsync_pakkaa.png" width="150"/>](img/qfieldsync_pakkaa.png)

tai valikosta **Lisäosat-\> QFieldSync-\> Pakkaa QFieldiä varten**. Oletuskansiona, johon QField-projekti paketoidaan, on käyttäjän kotikansion alla olevan QField-kansion Export-alikansio (Esim. C:\Users\käyttäjänimi\\QField\\Export). Valitse tai luo tyhjä kansio sopivaan sijaintiin ja paina **Luo** (Create). Prosessin valmistuttua QGISin karttaikkunan ylälaidan palkkiin tulee ilmoitus onnistumisesta ja kansiosijainti, jota klikkaamalla pääsee ko. sijaintiin.

Voit katsoa esimerkkiä alla olevasta videosta, joka tuotettiin Luonnonvarakeskukselle tuotetussa metsien koealoihin littyneessä QField-PoC-projektissa (vuonna 2024).

![Pakkaaminen QFieldiin](img/package_for_qfield_2.gif)

Jos et ole vielä kytkennyt omaa puhelinta tietokoneeseen esimerkiksi usb-kaapelilla, niin tee se. Käy sitten kopioimassa kaikki tiedostot (eli käytännössä em. kansio) jotka äsken loit lisäosan avulla ja siirrä ne puhelimeen sellaiseen sijaintiin, jonka muistat.

**Huom!**

Jos tietokoneella ei pääse näkemään yhtään tiedostoja puhelimella, niin avaa puhelimen näyttö ja salli tarvittaessa yhteyden muodostaminen. Saattaa olla tarpeen myös tarkistaa puhelimen asetuksista, että tiedostojen siirto on sallittu, eikä pelkkä lataus.

### Tiedostojen siirto

Siirtäminen tapahtuu esimerkiksi raahaamalla edellä luotu tiedostokansio (videossa nimellä testiversio1), tai kopioimalla tiedostoina kuten esimerkissä alla. Suosittelemme että luot uuden kansion jokaiselle projektille, jotta tiedostopolut ovat selkeitä.

![Tiedostojen siirto puhelimeen](img/tiedostojen_siirto.gif)
