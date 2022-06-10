---
layout: "default"
description: "Tietomallin muutokset versiosta toiseen"
id: "muutosloki"
---
# Muutosloki

## 10.6.2022

* Lisätty OsallistumisJaArviointisuunnitelma Yhteiset tietokomponentit -paketista (assosiaatio Rakennusjärjestys-luokkaan)
* Poistettu ErityispiirteinenAlue.erityispiirteenLaji ja sen koodisto AlueenErityispiirteenLaji, ei tunnistettua tarvetta.
* Uudelleennimetty RakennusjärjestyksenPykälä -> RakennusjärjestyksenMääräysryhmä. Pykälällä on vahva assosiaatio tiettyyn pykälänumeroon, mitä halutaan tässä välttää: numerointi voi poiketa saman Rakennusjärjestyksen eri versioissa ilman että ryhmä muuttuu (juokseva pykälänumerointi).
* Lisätty RakennusmääräyksenRyhmän-luokkaan rajoitus koskien jäseniä (vain RakennusjärjestyksenMääräys)