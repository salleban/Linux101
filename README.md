## Linux asennus
Installing Debian 11 in virtual machine

## Oracle VM VirtualBox Manager
Lähdetään luomaan uutta käyttöjärjestelmää VirtualBoxin avulla. Aloitettiin valitsemalla vasemmasta yläkulmasta Machine -> New... Tästä edettiin valitsemalla alhaalta painike Expert Mode. Tämän avulla lähdetään syöttämään ennakkotieto asennusta varten. 
Edetään järjestyksessä ja varmistetaan ennen kolmatta kohtaa, että varmasti on Debianin .iso tiedosto ladattu koneen tiedostoihin ja haetaan ISO Image kenttään oikea tiedosto. Seuraavalla välilehdellä Unattended Install syötetään käyttäjänimi sekä vahvat salasanat kirjautumista varten. Hardware välilehdellä syötetään Base Memory kohtaan 4000MB. 
Processors kohta pidetään sellaisenaan 1CPU. Hard Disk kohtaan Create a Virtual Hard Disk Now annetaan default vaihtoehto kohteelle, mutta syötetään 20 GB -> 60GB, jotta saadaan enemmän tilaa toiminnoille. Hard Disk File Type and Variant asetetaan VDI (VirtualBox Disk Image).

Tämän jälkeen tarkistetaan, että tiedosto polut on samat ylimmässä ja alimmassa välilehdessä, jolloin asennus alkaa toimimaan. Paina lopuksi Finish.

## Debian käynnistys
Ennen Debianin käynnistystä pitää mennä Settings -> Storage ja valita tämän jälkeen Storage Devices -> Controller: IDE, valitse Empty... ja tämän jälkeen lisätään Attributes kohtaan Optical Drive ja painetaan vetovalikon päässä olevasta cd painikkeesta oikea optinen asema debian-live.13.4.0... 
Sitten painetaan OK ja käynnistetään Debian. Varmista myös Settings -> General, että OS versio on sama kuin ISO tiedosto 64bit eikä 32bit. Muuten Debian ei lähde käyntiin.

## Debian aloitus
Käynnistyttyään valitaan Live system (amd64) ja odotellaan, että avautuu työpöytä näkymä.

## Debian Installation
Seuraavaksi valitaan työpöydän vasemmasta alakulmasta Install Debian painike ja aloitetaan asennus ja edetään seuraavasti: - Kieli, American English -> Next - Location, Suomi (Valitse painamalla Suomea kartasta) -> Next - Valitse vasemmasta valikosta Finnish ja Finnish (classic). 
Keyboard Model kohdassa pitäisi näkyä Generic 105-key PC (intl.) -> Next - Seuraavaksi valitaan Erase disk, jätetään alempaa Encrypt system valitsematta ja alimpana oleva valikko Boot loader location valitaan Master Boot Record... -> Next - Sitten täytetään käyttäjätietoja. Ensimmäiseen kohtaan oma nimi, toinen on kirjautumisnimi, tähän valitaan pienellä kirjoitettuna max 8 kirjainta/numeroa oleva yhdistelmä. 
Seuraavaan kohtaan älä laita omaa nimeäsi, yritä nimetä kone mahdollisimman anonyymisti. - Viimeisempänä valitse vahva salasana itsellesi, jokin sellainen, mitä et ole ennen käyttänyt. - Älä laita rastia Log in automatically without asking for the password. -> Next

Summary kohdassa on yhteenveto. Jos kaikki näyttää hyvältä, paina Install. Tämä saattaa viedä noin 10min aikaa. Nyt on aika tankata vesipullot!

Asentelun jälkeen ruutuun pamahtaa teksti All done. Valitaan rasti ruutuun Restart now(pitäisi olla automaattisesti valittuna) ja tämän jälkeen painetaan Done. 
Uudelleen käynnityksen jälkeen ikkunaan aukeaa kirjautumisikkuna. Tähän syötetään käyttäjätunnus ja salasana, jonka jälkeen olet valmis käyttämään Debiania!

## Loppu selvennys
Näin on saatu valmiiksi Debianin asennus VirtualBoxiin. Alun takkuilun jälkeen asennus oli äärimmäisen helppo. Mikäli ongelmia tulee, kannattaa hetkeksi pysähtyä ja miettiä vaihtoehtoisia ratkaisuja ongelmiin, näin kävi minun tapauksessani.



## Tiivistelmä OSS

OSS eli Open Source Software, sisältää avointa lähdekoodia, joka tarkoittaa sitä, että jokainen halutessaan voi tutkia, muuttaa tai parantaa koodia. 
Tarkoituksena on, että kehittäjät pääsevät tutkimaan muiden töitä ja tätä kautta saisivat enemmän ymmärrystä koodista, sen oppimisesta ja parantamisesta. 

Pääsy avoimeen lähdekoodiin auttaa myös yhteisöä kehittämään ja päivittämään ohjelmistoa, joka luetaan kaikkien eduksi, kun mietitään avointa koodia. 
Lähdekoodin näkyvyydellä myös innostetaan kehittäjiä kannustamaan ja kyseenalaistamaan ohjelmistoa. 
Avoin lähdekoodi on kaikille vapaa pelikenttä toteuttaa itseään ja rakentaa tai parannella ohjelmistoa, kun taas esimerkiksi yrityksillä saattaa olla heidän omanlaisensa ohjelmisto, mikä on yrityksen omaisuutta. Tällöin ohjelmisto ei ole avoin. 

Avointa lähdekoodia käyttävät esimerkiksi ihan tavalliset pulliaiset sekä ohjelmistojen kehittäjät, joiden tarkoitus on muokkaa ja parannella koodia. 
Vuonna 2025 tehdyssä raportissa kävi ilmi, että 97% tutkituista kaupallisista koodikannoista sisälsi avointa lähdekoodin koodia. 

Esimerkiksi Linux on yksi hyvä esimerkki avoimesta lähdekoodin ohjelmistosta.

## Tulevaisuuden ajatuksia.

Koen että avoimuus avoimessa lähdekoodissa lisää luottamusta turvallisuutta ajatellen. Moni haluaa kehittää turvallisuuttaan, varsinkin aikana, kun tekoäly on vielä melko uutta. 
Avoimuus on läpinäkyvää, ja luulen, että tulevaisuus tulee nostamaan entistä enemmän päätään tietoturvaa ajatellen. 

Digitaalista infraa kun ajatellaan, niin tähänkin liittyy omasta mielestäni turvallisuus ennen kaikkea. Valuutta pyörii sähköisenä ja käteinen raha alkaa pikkuhiljaa väistymään päivittäisestä elämästä. 
Ihmiset haluavat luottaa turvalliseen vahvistautumiseen sekä olla varmoja siitä, että päivittäiset ruokaostokset voidaan ostaa kortilla ilman pelkoa siitä, että jollakin on mahdollista ryöstää sinut. 

Näin ollen julkinen näkymä on parempi, kuin yksittäinen toimija, jonka alla on valta. 
