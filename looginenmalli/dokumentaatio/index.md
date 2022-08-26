---
layout: "default"
description: ""
id: "dokumentaatio"
status: "Ehdotus"
---

# Loogisen tason rakennusjärjestyksen tietomalli
{:.no_toc}

1. 
{:toc}

## Yleistä
Loogisen tason rakennusjärjestyksen tietomalli määrittelee tietomallimuotoisen rakennusjärjestyksen tietorakenteet ja sisällöt mahdollisimman riippumattomasti tietystä toteutusteknologiasta tai tiedon fyysisestä esitystavasta (esim. relaatiotietokanta, tietyn ohjelmointikielen tietorakenteet, XML, JSON). Tämä tietomallikuvaus mahdollistaa rakennusjärjestyksen tietojen tuottamisen, tallentamisen ja siirtämisen järjestelmästä toiseen ilman siten, että tietosisältö ja sen merkistys säilyy.

Tietomalli on kuvattu UML-kielellä ja sen graafinen luokkakaavioesitys on nähtävillä [omalla sivullaan](../uml/). Tietomallissa hyödynnetään luokkia {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/" title="RY-yhteisistä komponenteista" %}.

## Normatiiviset viittaukset
Seuraavat dokumentit ovat välttämättömiä tämän dokumentin täysipainoisessa soveltamisessa:

* [ISO 639-2:1998 Codes for the representation of names of languages — Part 2: Alpha-3 code][ISO-639-2]
* [ISO 8601-1:2019 Date and time — Representations for information interchange — Part 1: Basic rules][ISO-8601-1]
* [ISO 19103:2015 Geographic information — Conceptual schema language][ISO-19103]
* [ISO 19107:2019 Geographic information — Spatial schema][ISO-19107]
* [ISO 19108:2002 Geographic information — Temporal schema][ISO-19108]
* [ISO 19109:2015 Geographic information — Rules for application schema][ISO-19109]
* [ISO 19505-2:ISO/IEC 19505-2:2012, Information technology — Object Management Group Unified Modeling Language (OMG UML) — Part 2: Superstructure][ISO-19505-2]
* {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/" title="RY-yhteiset komponentit" %}

## Standardienmukaisuus
Looginen rakennusjärjestyksen tietomalli perustuu [ISO 19109][ISO-19109]-standardin yleinen kohdetietomalliin (General Feature Model, GFM), joka määrittelee rakennuspalikat paikkatiedon ISO-standardiperheen mukaisten sovellusskeemojen määrittelyyn. GFM kuvaa muun muassa metaluokat ```FeatureType```, ```AttributeType``` ja ```FeatureAssociationType```.  Kaikki tietokohteet, joilla on tunnus ja jota voivat esiintyä erillään toisista kohteista on määritelty kohdetyypeinä (stereotyyppi ```FeatureType```. Sellaiset tietokohteet, joilla ei ole omaa tunnusta ja jotka voivat esiintyä vain kohdetyyppien attribuuttien arvoina on määritelty [ISO 19103][ISO-19103]-standardin ```DataType```-stereotyypin avulla.

[ISO 19109][ISO-19109] -standardin lisäksi tietomalli perustuu muihin paikkatiedon ISO-standardeihin, joista keskeisimpiä ovat [ISO 19103][ISO-19103] (UML-kielen käyttö paikkatietojen mallinnuksessa), [ISO 19107][ISO-19107] (sijaintitiedon mallintaminen) ja [ISO 19108][ISO-19108] (aikaan sidotun tiedon mallintaminen).

### Rakennetun ympäristön yhteisistä komponenteista hyödynnetyt luokat

#### VersioituObjekti

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#versioituobjekti" title="Yhteiset tietokomponentit::Versioituobjekti" %}.

#### AlueidenkäyttöJaRakentamisasia

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#alueidenkäyttöjarakentamisasia" title="Yhteiset tietokomponentit::AlueidenkäyttöJaRakentamisasia" %}.

#### Toimija

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#toimija" title="Yhteiset tietokomponentit::Toimija" %}.

#### HallinnollinenAlue

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#hallinnollinenalue" title="Yhteiset tietokomponentit::HallinnollinenAlue" %}.

#### AlueidenkäyttöJaRakentamispäätös

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#alueidenkäyttöjarakentamispäätös" title="Yhteiset tietokomponentit::AlueidenkäyttöJaRakentamispäätös" %}.

#### Tietoyksikkö

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#tietoyksikkö" title="Yhteiset tietokomponentit::Tietoyksikkö" %}.

#### Tietoryhmä

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#tietoryhmä" title="Yhteiset tietokomponentit::Tietoryhmä" %}.

#### AlueidenkäyttöJaRakentamismääräys

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#alueidenkäyttöjarakentamismääräys" title="Yhteiset tietokomponentit::AlueidenkäyttöJaRakentamismääräys" %}.

#### OsallistumisJaArviointisuunnitelma

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#osallistumisjaarviointisuunnitelma" title="Yhteiset tietokomponentit::OsallistumisJaArviointisuunnitelma" %}.

#### RakennetunYmpäristönKohde

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#rakennetunympäristönkohde" title="Yhteiset tietokomponentit::RakennetunYmpäristönKohde" %}.

#### Lähtötietoaineisto

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#lähtötietoaineisto" title="Yhteiset tietokomponentit::Lähtötietoaineisto" %}.

#### Asiakirja

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#asiakirja" title="Yhteiset tietokomponentit::Asiakirja" %}.

#### Säädösviite

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#säädösviite" title="Yhteiset tietokomponentit::Säädösviite" %}.

#### AbstraktiSuureenArvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#abstraktiasuureenarvo" title="Yhteiset tietokomponentit::AbstraktiSuureenArvo" %}.

#### SuureenArvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#suureenarvo" title="Yhteiset tietokomponentit::SuureenArvo" %}.

#### EhdollinenSuureenArvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#ehdollinensuureenarvo" title="Yhteiset tietokomponentit::EhdollinenSuureenArvo" %}.

#### Ehto

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#ehto" title="Yhteiset tietokomponentit::Ehto" %}.

#### Ehtolause

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#ehtolause" title="Yhteiset tietokomponentit::Ehtolause" %}.

#### Suure

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#suure" title="Yhteiset tietokomponentit::Suure" %}.

#### OminaisuudenArvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#ominaisuudenarvo" title="Yhteiset tietokomponentit::OminaisuudenArvo" %}.

#### Ajanhetkiarvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#ajanhetkiarvo" title="Yhteiset tietokomponentit::Ajanhetkiarvo" %}.

#### Aikaväliarvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#aikaväliarvo" title="Yhteiset tietokomponentit::Aikaväliarvo" %}.

#### GeometriaArvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#geometriaarvo" title="Yhteiset tietokomponentit::GeometriaArvo" %}.

#### Koodiarvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#koodiarvo" title="Yhteiset tietokomponentit::Koodiarvo" %}.

#### NumeerinenArvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="Yhteiset tietokomponentit::NumeerinenArvo" %}.

#### Korkeuspiste

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#korkeuspiste" title="Yhteiset tietokomponentit::Korkeuspiste" %}.

#### NumeerinenArvoväli

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#numeerinenarvoväli" title="Yhteiset tietokomponentit::NumeerinenArvoväli" %}.

#### Korkeusväli

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#korkeusväli" title="Yhteiset tietokomponentit::Korkeusväli" %}.

#### Tunnusarvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#tunnusarvo" title="Yhteiset tietokomponentit::Tunnusarvo" %}.

#### Tekstiarvo

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#tekstiarvo" title="Yhteiset tietokomponentit::Tekstiarvo" %}.

#### AbstraktiVuorovaikutustapahtumanLaji

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#abstraktivuorovaikutustapahtumanlaji" title="Yhteiset tietokomponentit::AbstraktiVuorovaikutustapahtumanLaji" %}.

#### AbstraktiKäsittelytapahtumanLaji

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#abstraktikäsittelytapahtumanlaji" title="Yhteiset tietokomponentit::AbstraktiKäsittelytapahtumanLaji" %}.

#### AbstraktiAsianElinkaaritila

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#abstraktiasianelinkaaritila" title="Yhteiset tietokomponentit::AbstraktiAsianElinkaaritila" %}.

#### AbstraktiAsiakirjanLaji

Katso {% include common/moduleLink.html moduleId="yhteisetkomponentit" path="looginenmalli/dokumentaatio/#abstraktiasiakirjanlaji" title="Yhteiset tietokomponentit::AbstraktiAsiakirjanLaji" %}.

### Muulla määritellyt luokat ja tietotyypit

#### CharacterString

Kuvaa yleisen merkkijonon, joka koostuu 0..* merkistä, merkkijonon pituudesta, merkistökoodista ja maksimipituudesta. Määritelty rajapinta-tyyppisenä [ISO 19103][ISO-19103]-standardissa.

#### LanguageString

Kuvaa kielikohtaisen merkkijonon. Laajentaa [CharacterString](#characterstring)-rajapintaa lisäämällä siihen ```language```-attribuutin, jonka arvo on ```LanguageCode```-koodiston arvo. Kielikoodi voi [ISO 19103][ISO-19103]-standardin määritelmän mukaan olla mikä tahansa ISO 639 -standardin osa.

#### Number

Kuvaa yleisen numeroarvon, joka voi olla kokonaisluku, desimaaliluku tai liukuluku. Määritelty rajapintana [ISO 19103][ISO-19103]-standardissa.

#### Integer

Laajentaa [Number](#number)-rajapintaa kuvaamaan numeron, joka on kokonaisluku ilman murto- tai desimaaliosaa. Määritelty rajapintana [ISO 19103][ISO-19103]-standardissa.

#### Decimal

Laajentaa [Number](#number)-rajapintaa kuvaamaan numeron, joka on desimaaliluku. Decimal-rajapinnan toteuttava numero voidaan ilmaista virheettä yhden kymmenysosan tarkkuudella. Määritelty rajapintana [ISO 19103][ISO-19103]-standardissa. Decimal-numeroita käytetään, kun desimaalien käsittelyn tulee olla tarkkaa, esim. rahaan liityvissä tehtävissä.

#### Real

Laajentaa [Number](#number)-rajapintaa kuvaamaan numeron, joka on tarkkudeltaan rajoitettu liukuluku. Real-rajapinnan numero voi ilmaista tarkasti vain luvut, jotka ovat 1/2:n (puolen) potensseja. Määritelty rajapintana [ISO 19103][ISO-19103]-standardissa. Käytännössä esitystarkkuus riippuu numeron tallentamiseen varattujen bittien määrästä, esim. ```float (32-bittinen)``` (tarkkuus 7 desimaalia) ja ```double (64-bittinen)``` (tarkkuus 15 desimaalia).

#### TM_Object

Aikamääreiden yhteinen yläluokka, käytetään, mikäli arvo voi olla joko yksittäinen ajanhetki tai aikaväli. Määritelty luokkana [ISO 19108][ISO-19108]-standardissa. 

#### TM_Instant

Kuvaa yksittäisen ajanhetken 0-ulotteisena ajan geometriana, joka vastaa pistettä avaruudessa. Määritelty luokkana [ISO 19108][ISO-19108]-standardissa. Aikapisteen arvo on määritelty ```TM_Position```-luokalla yhdistelmänä [ISO 8601][ISO-8601-1]-standin mukaisia päivämäärä- tai kellonaika-kenttiä tai näiden yhdistelmää, tai muuta ```TM_TemporalPosition```-luokan avulla kuvattua aikapistettä. Viimeksi mainitun luokan attribuutti ```indeterminatePosition``` mahdollistaa ei-täsmällisen ajanhetken ilmaisemisen liittämällä mahdolliseen arvoon luokittelun tuntematon, nyt, ennen, jälkeen tai nimi.

#### TM_Period

Kuvaa aikavälin [TM_Instant](#tm_instant)-tyyppisten ```begin```- ja ```end```-attribuuttien avulla. Molemmat attribuutit ovat pakollisia, mutta voivat sisältää tuntemattoman arvon  ```indeterminatePosition = unknown``` -attribuutin arvon avulla annettuna. Määritelty luokkana [ISO 19108][ISO-19108]-standardissa.

#### URI

Määrittää merkkijonomuotoisen Uniform Resource Identifier (URI) -tunnuksen [ISO 19103][ISO-19103]-standardissa. URIa voi käyttää joko pelkkänä tunnuksena tai resurssin paikantimena (Uniform Resource Locator, URL).

#### Geometry

Kaikkien geometria-tyyppien yhteinen rajapinta [ISO 19107][ISO-19107]-standardissa. Tyypillisimpiä [ISO 19107][ISO-19107]-standardin Geometry-rajapintaa laajentavia rajapintoja ovat ```Point```, ```Curve```, ```Surface``` ja ```Solid``` sekä ```Collection```, jota käyttämällä voidaan kuvata geometriakokoelmia (multipoint, multicurve, multisurface, multisolid).

#### Point
Täsmälleen yhdestä pisteestä koostuva geometriatyyppi. Määritelty rajapintana [ISO 19107][ISO-19107]-standardissa.


## Tietomallin yleispiirteet

Kaavatietomallin UML-luokkakaaviot ovat saatavilla erillisellä [UML-kaaviot](../uml/)-sivulla.

## Luokat

### Rakennusjärjestys
Erikoistaa luokkaa [AlueidenkäyttöJaRakentamisasia](#alueidenkäyttöjarakentamisasia), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa käsitteen [Rakennusjärjestys](../../kasitemalli/#rakennusjärjestys).

**Assosiaatiot**

Roolinimi        | Kohde               | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
määräysryhmä     | [RakennusjärjestyksenMääräysryhmä](#rakennusjärjestyksenmääräysryhmä) | 0..* | rakennusjärjestykseen kuuluva määräysryhmä.
osallistumisJaArviointisuunnitelma | [OsallistumisJaArviointisuunnitelma](#osallistumisjaarviointisuunnitelma) | 0..* | Rakennusjärjestyksen osallistumis- ja arviointisuunnitelma.

### RakennusjärjestyksenHyväksymispäätös
Erikoistaa luokkaa [AlueidenkäyttöJaRakentamispäätös](#alueidenkäyttöjarakentamispäätös), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa käsitteen [Rakennusjärjestyksen hyväksymispäätös](../../kasitemalli/#rakennusjärjestyksen-hyväksymispäätös).

### RakennusjärjestyksenMääräysryhmä
Erikoistaa luokkaa [Tietoryhmä](#tietoryhmä), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa käsitteen [Määräysryhmä](../../kasitemalli/#määräysryhmä).

**Ominaisuudet**

Nimi             | Tyyppi              | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
pykälänumero     | [CharacterString](#characterstring) | 0..1  | määräysryhmälle mahdollisesti annettu pykälänumero. Voidaan käyttää ryhmien esittämiseen numerojärjestyksessä.
aihepiiri        | [RakennusjärjestyksenAihepiiri](#rakennusjärjestyksenaihepiiri) | 0..* | aihepiirit, joihin ryhmän määräykset liittyvät.
säädöviite       | [Säädösviite](#säädösviite) | 0..* | viittaus rakennusjärjestyksen ulkopuoliseen säädökseen, joka liittyy määräysryhmän määräyksiin.

**Assosiaatiot**

Roolinimi        | Kohde               | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
rakennusjärjestys     | [Rakennusjärjestys](#rakennusjärjestys) | 1 | rakennusjärjestys, johon määräysryhmä kuuluu.

Peritty assosiaatio ```jäsen``` on rajoitettu viittaamaan vain RakennusjärjestyksenMääräys-luokan tai sen aliluokkien objekteihin.

### RakennusjärjestyksenMääräys
Erikoistaa luokkaa [AlueidenkäyttöJaRakentamismääräys](#alueidenkäyttöjarakentamismääräys), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa käsitteen [Määräys](../../kasitemalli/#määräys).

**Ominaisuudet**

Nimi             | Tyyppi              | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
kohdistus        | [Kohdetyyppirajoitus](#kohdetyyppirajaus) | 0..* | määräyksen rajaus koskemaan vain tiettyjä alue- tai kohdetyyppejä.
säädöviite       | [Säädösviite](#säädösviite) | 0..* | viittaus rakennusjärjestyksen ulkopuoliseen säädökseen, joka liittyy määräysryhmän määräyksiin.

**Assosiaatiot**

Roolinimi        | Kohde               | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
rakennusjärjestys     | [Rakennusjärjestys](#rakennusjärjestys) | 1 | rakennusjärjestys, johon määräysryhmä kuuluu.

Peritty assosiaatio ```ryhmä``` on rajoitettu viittaamaan vain RakennusjärjestyksenMääräysryhmä-luokan tai sen aliluokkien objekteihin.


### MääräysSuunnittelutarvealueista
Erikoistaa luokkaa [RakennusjärjestyksenMääräys](#rakennusjärjestyksenmääräys), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa käsitteen [Määräys suunnittelutarvealueista](../../kasitemalli/#määräys-suunnittelutarvealueista).

**Ominaisuudet**

Nimi             | Tyyppi              | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
kaikkiAsemakaavoittamatonAlue        | boolean | 1  | määrätäänkö kaikki asemakaavoittamaton alue suunnittelutarvealueeksi.

**Assosiaatiot**

Roolinimi        | Kohde               | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
määrättyAlue     | [Suunnittelutarvealue](#suunnittelutarvealue) | 0..* | Suunnittelutarvealue, joka määräyksellä määrätään. Ei tarvitse antaa, mikäli kaikki asemakaavoittamaton alue on suunnittelutarvealuetta.

### ErityispiirteinenAlue
Erikoistaa luokkaa [RakennetunYmpäristönKohde](#rakennetunympäristönkohde), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa käsitteen [Erityispiirteinen alue](../../kasitemalli/#erityispiiteinen-alue).

### Suunnittelutarvealue
Erikoistaa luokkaa [RakennetunYmpäristönKohde](#rakennetunympäristönkohde), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa käsitteen [Suunnittelutarvealue](../../kasitemalli/#suunnittelutarvealue).

**Ominaisuudet**

Nimi             | Tyyppi              | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
voimassaoloAika  | [TM_Period](#tmperiod) | 0..1  | suunnittelualueen voimassaoloaika aikavälinä. Voi olla avoin kummasta tahansa päästä.

### KäytetytAvainsanat
Erikoistaa luokkaa [VersioituObjekti](#versioituobjekti), stereotyyppi: FeatureType (kohdetyyppi).

Kuvaa niiden avainsanojen joukon, jotka on liitetty yhteen tai useampaan rakennusjärjestysten määräyksiin.

**Ominaisuudet**

Nimi             | Tyyppi              | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
avainsana        | [MääräyksenAvainsana](#määräyksenavainsana) | 0..*    | yhteen tai usemapaan määräykseen liitetty avainsana.

### Kohdetyyppirajaus
Stereotyyppi: DataType (tietotyyppi).

Kuvaa yhdessä koodiston [Kohdetyyppi](#kohdetyyppi) arvojen kanssa käsitteen [Määräyksen aluetyyppirajoitus](../../kasitemalli/#määräyksen-aluetyyppirajoitus).

Käytetään kuvaamaan alue- tai kohdetyyppi, johon määräys voidaan kohdistaa ilman, että alueiden tai kohteiden geometriaa tai sijaintia on tarpeen määrittää osana rakennusjärjestystä. Näin rakennusjärjestyksen tietoja ei tarvitse päivittää, kun kohteena olevat halutun tyyppiset alueet tai kohteet (esim. tietyn rakennusluokituksen rakennukset tai käyttötarkoitusalueet) muuttuvat, lisäätyvät tai poistuvat.

Mikäli kohdistamiseen tarvitaan kohdetyypin lisäksi tarkennetta, käytetään ```tarkenne``` attribuuttia viittaamaan yhteen tai useampaan tarkoituksenmukaisen koodiston arvoon (esim. käyttötarkoitus tai rakennusluokka). 

**Ominaisuudet**

Nimi             | Tyyppi              | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
kohdetyyppi      | [Kohdetyyppi](#kohdetyyppi) | 0..*    | kohteen luokka.
tarkenne         | [Koodiarvo](#koodiarvo) | 0..*        | mahdollinen kohteen luokituksen tarkenne.
negaatio         | boolean             | 1               | kääntää merkityksen, jos arvo = true (muualle kuin kohdetyypin mukaiselle alueelle tai kohteeseen)

### MääräyksenAvainsana
Stereotyyppi: DataType (tietotyyppi).

Kuvaa käsitteen [Rakennusjärjestyksen määräyksen avainsana](../../kasitemalli/#rakennusjärjestyksen-määräyksen-avainsana).

**Ominaisuudet**

Nimi             | Tyyppi              | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
sanastonTunnus   | [URI](#uri) | 0..1                 | sanaston tunnus, josta avainsana on poimittu.
sanastonNimi     | [LanguageString](#languagestring) | 0..* | sanaston nimi, josta avainsana on poimittu.
sana             | [LanguageString](#languagestring) | 0..* | käytetty avainsana, mahdollisesti monikielisenä.

**Assosiaatiot**

Roolinimi        | Kohde               | Kardinaliteetti | Kuvaus
-----------------|---------------------|-----------------|------------------------------------
rakennusjärjestys| [Rakennusjärjestys](#rakennusjärjestys) | 1 | rakennusjärjestys, jonka määräyksiin avainsana liittyy
määräys          | [RakennusjärjestyksenMääräys](#rakennusjärjestyksenmääräys) | 0..* | määräys, johon avainsana on liitetty

### Koodistot

#### RakennusjärjestyksenAihepiiri
Stereotyyppi: CodeList (koodisto)

Laajennettavuus: [Laajennettavissa yksityiskohtaisemmilla koodiarvoilla](http://inspire.ec.europa.eu/registry/extensibility/narrower)

{% include common/codelistref.html registry="rakrek" id="rj-aihepiiri" name="Rakennusjärjestyksen aihepiiri" %}

#### MääräyksenKohdetyyppi
Stereotyyppi: CodeList (koodisto)

Laajennettavuus: [Ei laajennettavissa](http://inspire.ec.europa.eu/registry/extensibility/none)

{% include common/codelistref.html registry="rakrek" id="rj-maar-kohdetyyppi" name="Määräyksen kohdetyyppi" %}

#### RakennusjärjestyksenAvainsana
Stereotyyppi: CodeList (koodisto)

Laajennettavuus: [Laajennettavissa kaikilla tasoilla](http://inspire.ec.europa.eu/registry/extensibility/open)

{% include common/codelistref.html registry="rakrek" id="rj-avainsana" name="Rakennusjärjestyksen määräyksen avainsana" %}

#### RakennusjärjestyksenVuorovaikutustapahtumanLaji
Stereotyyppi: CodeList (koodisto)

Laajennettavuus: [Ei laajennettavissa](http://inspire.ec.europa.eu/registry/extensibility/none)

{% include common/codelistref.html registry="rakrek" id="rj-vv-tapahtumanlaji" name="Rakennusjärjestyksen vuorovaikutustapahtuman laji" %}

#### RakennusjärjestyksenKäsittelytapahtumanLaji
Stereotyyppi: CodeList (koodisto)

Laajennettavuus: [Ei laajennettavissa](http://inspire.ec.europa.eu/registry/extensibility/none)

{% include common/codelistref.html registry="rakrek" id="rj-ktapahtumanlaji" name="Rakennusjärjestyksen käsittelytapahtuman laji" %}

#### RakennusjärjestyksenElinkaaritila
Stereotyyppi: CodeList (koodisto)

Laajennettavuus: [Ei laajennettavissa](http://inspire.ec.europa.eu/registry/extensibility/none)

{% include common/codelistref.html registry="rakrek" id="rj-elinkaaritila" name="Rakennusjärjestyksen elinkaaren tila" %}

#### RakennusjärjestyksenAsiakirjanLaji
Stereotyyppi: CodeList (koodisto)

Laajennettavuus: [Ei laajennettavissa](http://inspire.ec.europa.eu/registry/extensibility/none)

{% include common/codelistref.html registry="rakrek" id="rj-asiakirjan-laji" name="Rakennusjärjestyksen asiakirjan laji" %}


[ISO-8601-1]: https://www.iso.org/standard/70907.html "ISO 8601-1:2019 Date and time — Representations for information interchange — Part 1: Basic rules"
[ISO-639-2]: https://www.iso.org/standard/4767.html "ISO 639-2:1998 Codes for the representation of names of languages — Part 2: Alpha-3 code"
[ISO-19103]: https://www.iso.org/standard/56734.html "ISO 19103:2015 Geographic information — Conceptual schema language"
[ISO-19107]: https://www.iso.org/standard/66175.html "ISO 19107:2019 Geographic information — Spatial schema"
[ISO-19108]: https://www.iso.org/standard/26013.html "ISO 19108:2002 Geographic information — Temporal schema"
[ISO-19109]: https://www.iso.org/standard/59193.html "ISO 19109:2015 Geographic information — Rules for application schema"
[ISO-19505-2]: https://www.iso.org/standard/52854.html "ISO/IEC 19505-2:2012, Information technology — Object Management Group Unified Modeling Language (OMG UML) — Part 2: Superstructure"