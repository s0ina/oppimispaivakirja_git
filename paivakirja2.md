# Oppimispäiväkirja: Hajautettu git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet, jotka vaikuttivat tehtävän suorittamiseen?__

Osion tehtävissä vaikeinta oli päästä alkuun. Paikallisen master-haaran vieminen GitHubiin tuotti aluksi päänvaivaa, sillä en ymmärtänyt miksi toiminto ei onnistu – yritin siis viedä master-haaraa tyhjänä etärepositorioon. Pienen selvittelyn ja googlailun jälkeen opin, että master-haaran voi viedä etärepositorioon tekemällä jokin commitin. Tämän jälkeen tehtävä sujui ongelmitta, ja etenin vaihe vaiheelta tehtävänannon mukaisesti. Tehtävässä oli hyvää kertausta perustoiminnoista.

## Osiossa käyttämäni Git-komennot

| Komento | Kuvaus |
| --------| ------ |
| git init | luo kansioon tyhjän repositorion |
| git branch -a | listaa olemassaolevat kehityshaarat |
| echo  | luo tekstitiedoston|
| git checkout (master)  | luo uuden kehityshaaran |
| git push -u origin (master)  | vie paikallisen kehityshaaran muutokset etärepositorion kehityshaaraan|
| git remote add origin | määrittelee etärepositorion|
| git fetch | hakee etärepositorion muutokset |
| git merge origin/master | yhdistää paikallisen ja etärepositorion muutokset |