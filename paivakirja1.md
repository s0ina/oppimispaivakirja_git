# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

Perustoiminnot, kuten clone, add, commit ja push olivat entuudestaan tuttuja ja tuntuivat helpoilta. Kohtasin hieman ongelmia edellisten versioiden palauttamisessa checkout-toiminnolla, sillä olin jostain syystä siirtynyt hakemistossa repositorion ulkopuolelle. Tehtävä 3 tuntui aluksi vähän vaikealta ha mottaa, mutta pääsin lopulta kärryille, kun etenin asia kerrallaan ja yritin muutaman kerran. Uuden haaran luominen ei heti onnistunut current branch has no upstream branch -errorin vuoksi, mutta googlettamalla tähän löytyi ratkaisu. Muutoin tehtävä 4 onnistui hyvin.

## Osiossa käyttämäni Git-komennot
| Komento     | Kuvaus |
| ----------- | ----------- |
| git clone| kopioi olemassa olevan repositorion|
| git rm | poistaa tiedoston|
| git mv | uudelleennimeää tiedoston |
| git add| lisää paikalliset muutokset tallennettaviksi|
| git status |näyttää verionhallintaan valmistellut muutokset|
| git commit | valmistelee tehdyt muutokset verionhallintaan, sen yhteydessä lisätään myös commit -viesti |
| git push | tallentaa muutokset verionhallintaan |
| git log | näyttää viimeisimmät tallennukset |
| git checkout | vaihtaa aikaisempaan tallennukseen tai toiseen kehityshaaraan |
| git revert | palauttaa viimeksi tallennetun version |
| git config --global push.default current | luo uuden haaran myös etärepositoriion |
| git merge | yhdistää kehityshaarat |
| git switch | vaihtaa kehityshaaraa |