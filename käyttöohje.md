# Kisan lisääminen

Lataa desktop client ja asenna dependencyt:
```
> git clone git@github.com:f1-2019-results/desktop-client.git
> cd desktop-client
> npm i
```

Laita F1 2019 pelin asetuksista UDP telemetria päälle, porttiin 20777 (oletusasetus) ja käynnistä desktop-client komennolla `npm start`.
Aloita kisa F1 2019 pelissä. Kisan jälkeen konsolin pitäisi näyttää tältä:
```
Waiting for race start
Race started
Race ended
Race results available at https://f1-2019-results.github.io/#/race/16ea1e83-96f9-4068-957f-e3480748d7ec
```

# Kisan tuloksien katselu

Tuloksia näkee osoitteesta https://f1-2019-results.github.io/#/
<img src="https://i.gyazo.com/c633bf7c20bb2f25b9804c6657c55f92.png">
View race linkkiä painamalla pääse kisan tuloksiin
<img src="https://i.gyazo.com/3796a661f7a876ed24c7022ee3221490.png">
"Position graph" tabissa näkee graafin kilpailijoiden positiosta kilpailun aikana. "P" markkeri tarkoittaa että kilpailija on käynyt varikolla alkavalla kierroksella.
<img src="https://i.gyazo.com/3fcfb4ea91725cdaea520550ac52a70f.png">
