---
layout: "default"
description: "Tietomallin muutokset versiosta toiseen"
id: "muutosloki"
---
# Muutosloki

## 26.8.2022
* Lisätty uusi attribuutti ```RakennusjärjestyksenMääräys.määräysteksti```, jotta kuhunkin määräykseen liitettävää määräystekstiä varten ei tarvitse käyttää ```RakennusjärjestyksenMääräys.ominaisuus``` -attribuuttia suureen arvona "Määräysteksti".
* Muutettu avainsanoituksen mallia siten, että määräykseen liitetyt avainsanat eivät ole osa RakennusjärjestyksenMääräys-luokkaa, vaan määräyksiin viitataan ulkopäin MääräyksenAvainsana-tietotyypin kautta. Näin hyväksyttyyn rakennusjärjestyksen määräykseen voidaan myöhemmin liittää uusia avainsanoja tai poistaa niintä muuttamatta itse määräysten tietosisältöä. Lisätty uusi kaavio "Avainsanat" kuvaamaan avainsanojen käyttöä.

## 18.8.2022
* Lisätty uusi DataType Avainsana, joka mahdollistaa avainsanojen käytön myös RakennusjärjestyksenAvainsana-koodiston ulkopuolelta. RakennusjärjestyksenMääräys.avainsana-attribuutti on nyt tyypiltään Avainasana. Lisätty rajoite RakennusjärjestyksenMääräys-luokan perittyyn attribuuttiin ```ryhmä```: se voi nyt olla tyypiltään vain RakennusjärjestyksenMääräysryhmä tai sen perillinen.
* Lisätty koodistojen sanastolinkit CodeList-luokkien ```vocabulary```-tageiksi.

## 17.8.2022
* Poistettu koodistot AlueenErityispiirteenLaji ja OsallisenHuomionninLaji, ja vastaavasti niitä käyttäneet attribuutit RakennusjärjestyksenMääräys.vaadittuOsallisenHuomiointi ja EritysipiirteinenAlue.erityispiirteenLaji.
* Lisätty UML-luokkien tekstimuotoinen dokumentaatio.
* Lisätty käsitteiden kuvaukset.

## 15.8.2022
* Lisätty uusi luokka Kohdetyyppirajaus (DataType), uudelleennimetty koodisto MääräyksenAluetyyppirajoitus -> Kohdetyyppi. Uudelleennimetty ja tyypitetty attribuutti RakennusjärjestyksenMääräys.aluetyyppirajoitus:MääräyksenAluetyyppirajoitus -> RakennusjärjestyksenMääräys.kohdistus:Kohdetyyppirajaus. Uusi rakenne mahdollistaa myös ulkoisten koodistojen (esim. asemakaavan kaavamääräyslaji/käyttötarkoitus tai Rakennusluokitus) käytön määräysten kohdistamiseen.

## 16.6.2022
* Lisätty takaisin ErityispiirteinenAlue.erityispiirteenLaji ja sen koodisto AlueenErityispiirteenLaji, mahdollinen tarve (maanlämpö, porakaivot yms.)
* Lisätty attribuutti RakennusjärjestyksenMääräysryhmä.pykälänumero

## 10.6.2022

* Lisätty OsallistumisJaArviointisuunnitelma Yhteiset tietokomponentit -paketista (assosiaatio Rakennusjärjestys-luokkaan)
* Poistettu ErityispiirteinenAlue.erityispiirteenLaji ja sen koodisto AlueenErityispiirteenLaji, ei tunnistettua tarvetta.
* Uudelleennimetty RakennusjärjestyksenPykälä -> RakennusjärjestyksenMääräysryhmä. Pykälällä on vahva assosiaatio tiettyyn pykälänumeroon, mitä halutaan tässä välttää: numerointi voi poiketa saman Rakennusjärjestyksen eri versioissa ilman että ryhmä muuttuu (juokseva pykälänumerointi).
* Lisätty RakennusmääräyksenRyhmän-luokkaan rajoitus koskien jäseniä (vain RakennusjärjestyksenMääräys)