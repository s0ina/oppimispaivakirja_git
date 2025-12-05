# Oppimispäiväkirja: Git projektissa

__Mitä hyötyä voisi olla versionhallinnasta, jos kehität projektia yksin?__

Vaikka projektia kehittää yksin, voi olla omaa työtä selkeyttävää pitää valmiit toiminallisuudet ja keskeneräiset osat erillään toisistaan. Verionhallintaa voi siis käyttää oman työn organisointiin. Kehityshaarat mahdollistavat myös erilaisten lähestymistapojen kokeilun ilman, että aikaisempia tiedostoja täytyy poistella tai siirellä. Ei myöskään tarvitse huolehtia koko projektin hajoamisesta, vaikka jokin kokeilu menisikin hieman mönkään.

__Mitä hyötyä voisi olla versionhallinnasta, jos projektissa on useita kehittäjiä?__

Verionhallinta helpottaa myös ryhmätyöskentelyn organisointia. Jokainen voi hoitaa omat sovitut tehtävänsä ja testata ratkaisujaan omassa eristetyssä ympäristössä, eikä koko projektin hajoamisesta tarvitse huolehtia. Versionhallinan avulla tiimi voi myös seurata mitä on tehty, kenen toimesta ja miksi. Se helpottaa lisäksi koodikatselmointeja ja valmiiseen versioon eksyy epätodennäköisemmin bugeja, jos myös joku toinen testaa muutokset omassa ympäristössään ennen main/master-kehityshaaraan tallentamista.

__Miten järjestäisit projektitiimin versionhallinnan 3-4 hengen ohjelmistoprojektikurssilla? Laadi tiimiläisille lyhyt ohje, miten projektissa toimitaan.__

Ehdottaisin tähän feature-branch tekniikkaa, sillä se on osoittautunut varsin toimivaksi omissa projektitöissäni.
Etärepositorioon luodaan kaksi kehityshaaraa – main ja develop. Mainissa pidetään yhdessä valmiiksi todetut ominaisuudet, ja sinne viedään muutoksia ainoastaan develop-haaran kautta. Uusimmat muutokset haetaan develop-haarasta, ja viedään develop-haaraan feature-haarojen kautta. Feature-haaran voi luoda esimerkiksi suoraan issuesta GitHub-projects-taululta.
Kun kehittäjä on testannut muutokset omassa ympäristössään, feature-haarasta voi tehdä pull requestin develop-haaraan. Jonkun toisen ryhmäläisen on hyvä testata ominaisuus omassa ympäristössääm ja ehdottaa tarvittaessa muutoksia. Kun yksi tai useampi ryhmästä on hyväksynyt muutokset, voi featuren mergetä develop-haaraan. Feature-haaran voi tämän jälkeen poistaa.
Muutokset develop-haarsta mainiin tehdään projektin aikataulusta riippuen esimerkiksi kerran viikossa. Koko ryhmä osallistuu koodikatselmointeihin ja varmistaa, että mainiin viedyt muutokset toimivat omissa ympäristöissä. Näin main-haaraan ei todennäköisesti eksy rikkinäisiä ominaisuuksia, ja koko tiimi pysyy projektista ajan tasalla.

__Kommenttini opintojaksosta, esim. sisällöstä, materiaalista, työmäärästä, hyödyllisyydestä, työmäärästä. Mitä toivoisit olevan enemmän, mitä vähemmän?__

Opintojakson työmäärä oli mielestäni sopiva ja materiaalit todella kattavat. Koin opintojakson sisällön hyödylliseksi, sillä verionhallinnan opettellu jää usein toisijaiseksi projektia työstäessä, ja melko yksinkertaisetkin ongelmat saattavat silloin tuntua turhauttavilta. Oli hyödyllistä keskittyä perustoimintoihin, jotka kuitenkin rakentuivat oikean projektin ympärille. Kiitos kurssista!
