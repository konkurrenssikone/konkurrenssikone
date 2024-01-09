# Konkurrenssikone

**A summary in English is available at the end of this readme file.**

**Konkurrenssikone** on useissa tuomioistuimissa käytössä oleva JavaScript-sovellus, joka määrittää [rikoslain 7 luvun 6 §:n](https://www.finlex.fi/fi/laki/ajantasa/1889/18890039001#L7P6) soveltamiseen liittyvät ns. konkurrenssiryhmät noudattaen ennakkopäätöksistä [KKO 1972 II 5](https://finlex.fi/fi/oikeus/kko/kko/1972/19720005t) ja [KKO 2004:130](https://finlex.fi/fi/oikeus/kko/kko/2004/20040130) johdettua algoritmia. Konkurrenssikone on julkistettu, jotta yleisö voi perehtyä ohjelman lähdekoodiin ja toimintaperiaatteeseen sekä konkurrenssialgoritmin automatisoinnin toteutukseen.

Sovellus on ladattavissa oheisena HTML-tiedostona, joka toimii yleisimmillä selaimilla. Käyttäjä syöttää konkurrenssikoneeseen PDF-muotoisen rikosrekisteriotteen tekstisisällön, ja sovellus antaa vastauksena HTML-muotoisen tulosteen, josta konkurrenssiryhmien määräytyminen ilmenee. Tulosteeseen sisältyy myös mm. graafinen esitys rikosrekisteriotteella olevista tuomioista.

Konkurrenssikone on koekäyttöön tarkoitettu beeta- eli testiversio, jonka käyttö tapahtuu omalla vastuulla. Minkäänlaista teknistä tukea tai käyttöopastusta ei voida tarjota. Koekäytössä voi hyödyntää oheista rikosrekisteriotteen mallikappaletta sekä *Demo*-painikkeesta aktivoitavaa esittelytoimintoa, joka muodostaa fiktiivisiin tietoihin perustuvan esimerkin konkurrenssikoneen tulosteesta. PDF-tiedostosta siirrettävien tietojen luenta on testattu PDF-XChange- ja Acrobat Reader -sovelluksilla.

Konkurrenssikone sisältää käyttöohjeet sekä yleistä tietoa sovelluksen toiminnasta. Sovelluksen toimintalogiikka on selostettu yksityiskohtaisesti lähdekoodin kommenteissa. Lisätietoa konkurrenssikoneesta on kahdessa artikkelissa, joista toinen on julkaistu [Helsingin hovioikeuden yliopistopainotteisen laatuhankkeen julkaisussa 2021](https://oikeus.fi/material/collections/20210407093422/7PNsJ7hZR/Valittuja_kysymyksia_rikos-_prosessi-_ja_vahingonkorvausoikeudesta_I_2021.pdf) (s. 419—480, open access) ja toinen [Defensor Legis -aikakauskirjassa 1/2022](https://www.edilex.fi/defensor_legis/1000490008.pdf) (s. 106—131, Edilex/maksumuuri).

Konkurrenssikoneen on kehittänyt Helsingin hovioikeudessa hovioikeudenneuvos Juha Terho (sähköpostiosoite muotoa etunimi.sukunimi@oikeus.fi).

## Tulevia muutoksia

- **Versio 0.999 (arvioitu julkaisu 2022)**
    - Tuomioiden lisäämis- ja muokkaamistoiminto.
    - Toiminto samana päivänä annettujen tuomioiden keskinäisen järjestyksen muuttamiseksi.
    - Varoitus tilanteista, joissa riittävä seuraamus -tuomio määrittyy konkurrenssin katkaisevaksi.
    - Ns. keskipitkä malli konkurrenssilausunnoille (kohdittain eritellyt lausunnot, joissa kukin huomioon otettava tuomio mainitaan vain kerran).
    - Pitkän mallin konkurrenssilausuntojen ulkoasun/sanamuodon mahdolliset täsmennykset.
    - Toiminto, joka määrittää, miltä osin eri tuomiot voivat vaikuttaa konkurrenssiryhmien määräytymiseen.
    - Varoitus tilanteista, joissa rikosrekisterin osaote ei ole riittävä.
    - Muutoksenhakujen esittäminen konkurrenssikaaviossa (käyttäjän valinnan mukaan).
	- Demo-toiminnon kehittäminen: aikaisempien tuomiopiirijakojen lisääminen ja liikkuvien pyhäpäivien huomioon ottaminen.
    - Erillinen toiminto vapaudenmenetysaikojen laskemiseksi.
    - Ulkoasun uudistaminen.
	- Erillisen IE-tuen mahdollinen poistaminen.
	- Lähdekoodin stilisointeja.
- **Laajempia uudistuksia (ei aikataulua)**
	- Vaihtoehtoinen malli rikosrekisteriotteen tietojen siirtämiseksi konkurrenssikoneeseen (sis. ruotsinkieliset rikosrekisterimerkinnät).
	- Konkurrenssiryhmien määräytymistä koskevien perustelujen automaattinen luominen.

## English Summary

**Konkurrenssikone** is a standalone JavaScript app which is used by several courts of law in Finland to analyze the criminal records of defendants. This is a public beta release for testing purposes and is provided ”as is”. Use at your own risk. The user interface, source code (variable and function names, comments etc.) and the reports generated by the app are in Finnish. To get a sample report with randomly generated data, first click *Demo* and then click *Luo ja analysoi mallirikosrekisteri alla olevien asetusten mukaan*.
