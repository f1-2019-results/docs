# Vaatimusmäärittely

## Sovelluksen tarkoitus

Kerätä telemetriaa eri ajosimulaattoreista ja peleistä ja näyttää siitä mielenkiintoista statistiikkaa web clientissä. Lisäksi käyttäjät voivat luoda "sarjoja", eli kokonaisuuksia joihin kuuluu useampi kisa. Sarjoista voidaan mm. laskea kuljettajien pisteitä ja muuta statistiikkaa. Sovelluksen tulisi tukea useita simulaattoreita/pelejä, mutta aluksi F1 2019 riittää. 

Toimintoja ensimmäisessä versiossa:
* Komentorivipohjainen desktop client pelin telemetrian lukemiseen ja serverille lähettämiseen
* Rekisteröityminen/kirjautuminen web clientissä
* Kisojen statistiikkaa: sijoitukset (per kierros), kierrosajat.
* Mahdollisuus luoda sarjoja jotka koostuu useammasta kisasta. Sisältää ainakin sarjaan kuuluvat kisat, kisoista saadut pisteet.

## Jatkokehitysideoita
* Electron pohjainen desktop client telemetrian lukemiseen.
* Tuki useammalle simulaattorille/pelille. mm. Assetto Corsa, Project Cars
* Tuki konsolipeleille. Käytännössä pitäisi olla helppoa, koska konsolipelit streamaa telemetriaa ihan samalla tavalla kun pc pelit. Pitää tutkia. (telemetriaa keräävä sovellus toki pitää ajaa tietokoneella)
* Tarkempaa telemetriaa (mm. nopeus, kaasu, jarru, sijanti radalla yms.). Yksi ongelma datan paljous. F1 2019 dataa tulee noin 4-5MB minuutissa, eli puolen tunnin kisa olisi varmaan yli 100MB. Tavallaan olisi hyvä juttu tallentaa koko dumppi serverille sen sijaan että parsitaan dumppi clientillä, koska sitten dumpit voitaisiin parsia uudelleen tarvittaessa. Pitää tutkia miten hyvin dumppia saisi pakattua, mahdollisesti jonkinlaisen esikäsittelyn kanssa.
* Telemetriaa myös muista kuin kisoista. (time trial, practice)
* Manuaalisesti annettavat rangaistukset kisan jälkeen (mm. aika- tai sijarangaistus)
* Aika-ajojen ja harjoitusten tallennus.
